---
layout: page
title: Checking the mark
---

Every sound Aftervoice plays carries a mark that says a machine made it. This page says what
the mark is, how to check it yourself, and — because it matters more than the rest — what it
cannot do.

You do not need us for any of this. The detector is the same code the app uses, published
under a permissive licence, and the reference patterns it compares against do not depend on
any secret. Two people running it on the same file get the same answer.

## What the mark is

A spread-spectrum watermark in the sound itself, not a tag attached to the file.

The audio is cut into overlapping windows of 2048 samples at 48 kHz. In each window, a
pseudo-random pattern decides which frequency bins are nudged slightly louder and which
slightly quieter — about 0.7 dB, in a band where a small change is least likely to be heard
and least likely to be destroyed. The pattern comes from a fixed key, so a detector can
re-derive it and ask how strongly a file agrees with it.

Because it lives in the audio, it survives what a file goes through: sharing, re-encoding to a
lossy format, a change of container, renaming, and a trim down to a few seconds.

## How a file is judged

Not against a fixed number. Against itself.

The detector correlates the file with our pattern, and then correlates the same file with
thirty-one decoy patterns that are not ours. Whatever the audio has of its own — a musical
chord, a repeating loop, a tone — shows up in the decoys too, and what is left after that
comparison is the mark or nothing. The result is a z-score: how far our pattern stands out
from the decoys, in standard deviations.

The threshold is **5**. Above it, the file is marked. Below, it is not.

That design replaced an earlier one that compared against a constant, and it had to. Measured
across six kinds of signal, unmarked audio was reaching a hundred standard deviations against
a constant: a harmonic chord correlates strongly with *any* fixed pattern, and by the same
amount every time, which against a constant looks exactly like a watermark.

## What has been measured

Two measurements, made independently, and the interesting thing is that they agree.

**Synthetic signals**, 960 judgements — white noise, our own noise bed, brown noise, a harmonic
stack, a sweep, and a speech-shaped signal, under four different keys.

**Real recorded audio nobody here made**, 202 judgements: 65 produced music tracks, each judged
whole and again as a ten-second clip, and 72 utterances of recorded speech from LibriSpeech's
public-domain validation set.

| | worst score | read as marked |
|---|---|---|
| synthetic, 960 judgements | 3.07 | none |
| music, whole | 2.97 | none |
| music, ten-second clip | 3.18 | none |
| recorded speech | 0.76 | none |
| **threshold** | **5.0** | |

The two worst cases, 3.07 and 3.18, come from completely different material and land in the
same place. That is what says the synthetic number was not flattering itself.

Two things those numbers do not say. Produced music sits at a mean of +1.1 rather than zero, so
the margin is about 3.6 standard deviations of that distribution rather than the five the
absolute figure suggests. And the sample is one music library and one speech corpus; a wider
one is more work, not a correction.

On our own files: a clean noise bed reads −0.4, the same bed marked reads 12.0, and a recording
made on a phone during an actual session reads 9.6.

## What the mark cannot do

**It is not a signature and it is not an identifier.** It carries no phone identifier, no
session identifier, no installation identifier, no timestamp. It says one thing: a machine made
this audio. It cannot tell you which copy of the app, or whose.

**It does not survive everything.** Heavy pitch shifting, time stretching, or a strong
band-stop filter across the carrying band will remove it. It is a mark of origin, not
tamper-proofing, and anyone determined to strip it can.

**It cannot ride on a signal that has nothing to modulate.** A nearly pure tone — a chord of
sine waves, a sweep, a buzz — will not carry it, because there is nothing in the carrying band
to nudge. This is a fact about those signals rather than a fault in the mark: Aftervoice always
plays over a broadband noise bed, and that is what carries it.

**Absence of the mark proves nothing.** A file with no mark is a file with no mark. It may be
someone else's recording, or ours after processing that removed it. Only its presence is
evidence, and only of one thing: this audio was generated.

## Running it

The detector is [`evp-mark`](https://github.com/samjanny/evp-mark), MIT OR Apache-2.0.

```sh
git clone https://github.com/samjanny/evp-mark
cd evp-mark
cargo run --release --bin detect-mark -- path/to/file.wav
```

It prints the score and a verdict, and sets its exit status to match: 0 marked, 1 not marked or
too little audio to say, 2 unreadable. `--json` gives the same answer to anything that has to
act on it. Any WAV, or any format your system can decode to one, will do; the file does not have
to come from us, and running it on audio that is not ours is the best way to see what a negative
answer looks like.

Nothing in it reaches the network, and the pattern it compares against is derived from a key
printed in the source. Two people running it on the same file get the same answer without either
of them asking us for anything — which is the only sense in which a detector can be public.

## Why the mark exists

Article 50 of the European AI Act asks that synthetic audio be marked in a machine-readable
way, and detectable as artificially generated, as far as is technically feasible. This page is
our answer to "as far as is technically feasible": the numbers above are what we measured, and
the limits above are the ones we found.

There is also a reason that has nothing to do with the law. Aftervoice makes sounds that people
listen to closely, looking for meaning. Audio like that should be able to say what it is, years
later, to someone who was not there.

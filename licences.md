---
layout: page
title: Licences
---

The app names all of this on its own Informazioni screen, offline, because a licence page that
can fail to load is not a licence page. This page is the same list, for anyone who wants to
read it before installing.

## The voices

The voices are neural models trained by other people. The licences on the ones that ship ask to
be told whose they are, and here is whose. Each downloaded voice pack carries its own
attribution file, and the app reads the credits from the pack rather than from a list someone
has to remember to update.

| Voice | Language | Licence |
|---|---|---|
| `it_IT-giorgio` | Italian | CC BY 4.0 — model and dataset both declare it |
| `it_IT-aurora-medium` | Italian | CC BY 4.0 — model and dataset both declare it |
| `en_US-libritts-high` | English | CC BY 4.0 — trained on LibriTTS (openslr.org/60) |
| `es_ES-carlfm-x_low` | Spanish | MIT model — trained from scratch on a public-domain corpus |
| `es_ES-carlfm-x_low` | Brazilian Portuguese fallback | Same MIT model and public-domain corpus; shared with Spanish |
| `fr_FR-mls-medium` | French | CC BY 4.0 — trained from scratch on Multilingual LibriSpeech |
| `de_DE-mls-medium` | German | CC BY 4.0 — trained from scratch on Multilingual LibriSpeech |

A voice is only shipped when both the model and the dataset behind it permit commercial use. A
model whose dataset is share-alike is not shipped, whatever its quality, because the app itself
is not.

## The engine

**ONNX Runtime** 1.29.0, MIT, Copyright Microsoft Corporation. Every voice model runs on it.

## The software

The app is built on the work of others: the Android and Jetpack libraries under Apache-2.0, JNA
under Apache-2.0, Google's asset delivery library under the Play Core SDK Terms of Service, and
about a hundred and fifty Rust crates, mostly MIT or Apache-2.0. The complete list, grouped by
licence with the full text of each, is in the app under **Impostazioni → Informazioni e
licenze**.

## Ours

**[`evp-mark`](https://github.com/samjanny/evp-mark)**, the watermarking and detection crate, is
published under MIT OR Apache-2.0 so that anyone can verify our audio without our help. See
[Checking the mark](detector.html) for what it does and how to run it.

The rest of the app is not open source.

This site's own text is CC BY 4.0.

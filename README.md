# The public Aftervoice site

These files are the source of `https://aftervoice.altrovelabs.net/`. They stay here until the
public `aftervoice-site` repository exists: the app core remains private while the policy,
support information and detector documentation remain public and versioned.

```
index.md             product page
support.md           contact, reporting and common questions
detector.md          what the mark is and how to check it
licences.md          voices, engine and software
privacy/*.md         privacy policy in all six interface languages
_config.yml          GitHub Pages configuration
CNAME                stable custom domain
.github/…/pages.yml  Pages build and deployment
```

## Publishing

The public repository uses the Pages workflow in `.github/workflows/pages.yml`. Configure its
custom domain and add a DNS `CNAME` record from `aftervoice.altrovelabs.net` to
`samjanny.github.io`. The Android app and Play Console use these stable URLs:

- `https://aftervoice.altrovelabs.net/privacy/it.html`
- `https://aftervoice.altrovelabs.net/support.html`

The public contact is `support@altrovelabs.net` and the data controller is Altrove Labs. Verify
that the mailbox receives mail before publishing.

The current watermark strength is approximately 0.7 dB (`alpha = 0.085`). Repeat the listening
gate and update the measured examples whenever that value changes.

## Why the text is checkable

Every claim in the policy corresponds to a property of the release: permissions in the
manifest, backup rules in `res/xml/`, storage under `filesDir`, and the mark applied before both
speaker and recorder. If reporting is added, the privacy policy and Play Data Safety answers
must describe precisely what the report sends and how long it is retained.

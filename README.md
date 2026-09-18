# ishomnikov.github.io

Two static pages. They exist for exactly one reason, and it is not a website.

## Why this repo exists

Google's OAuth consent screen will not let you **publish** an app without an
**application homepage URL** and a **privacy policy URL**. It also requires the
authorized domain to be one you effectively own — `sites.google.com`, a Notion
page or a Gist are all rejected. A `*.github.io` subdomain qualifies, because
`github.io` is on the Public Suffix List.

So these two pages are the minimum artifact needed to register a personal OAuth
client with Google:

- `index.html` → https://ishomnikov.github.io/
- `privacy.html` → https://ishomnikov.github.io/privacy.html

They back the OAuth app **"Starfox"** (Google Cloud project `starfox-508922`),
which authorises a personal automation harness on a single Mac Mini to reach
Google Drive and Gmail for one dedicated account.

## Do not delete this repo

Removing it breaks the URLs on a published OAuth consent screen. That does not
fail loudly — it surfaces later as authorisation problems on a tool that had
been working for months.

## The privacy policy is a real promise

It states that all processing happens locally on one owned machine, that
credentials are stored locally with restricted permissions, and that nothing is
transmitted to a server the author operates, sold, shared, or used for training.

All of that is true today. **If the architecture changes — a hosted component, a
third-party relay, anything that moves data off the machine — the page must be
updated to match.** It is a public statement, not boilerplate.

## Housekeeping

The pages currently title themselves "iVault Harness" while the registered app
is named "Starfox". Cosmetic, and harmless unless the app is ever submitted for
Google verification, which would flag the mismatch.

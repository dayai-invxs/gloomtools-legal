# gloomtools-legal

Public privacy policy and support pages for the **GloomTools** iOS app, served
via GitHub Pages.

This repo is public only so the pages are reachable — Apple requires a publicly
accessible privacy policy URL for App Store review. The app's source code lives
in a separate private repository.

## Pages

| File | URL |
|---|---|
| `index.md` | `https://dayai-invxs.github.io/gloomtools-legal/` |
| `privacy.md` | `https://dayai-invxs.github.io/gloomtools-legal/privacy` |
| `support.md` | `https://dayai-invxs.github.io/gloomtools-legal/support` |

## Editing

Pages are Markdown with Jekyll front matter, rendered by GitHub Pages using the
`jekyll-theme-minimal` theme set in `_config.yml`. Push to `main` and the site
rebuilds automatically, usually within a minute.

Update the effective date in `privacy.md` whenever the policy changes
materially.

## Keeping the policy true

The policy claims the app collects nothing and makes no network requests. That
is currently accurate: the app imports only Foundation, SwiftUI, and
Observation, requests no permissions, and writes a single JSON file to its own
Documents directory. Adding any SDK, analytics, crash reporter, or sync feature
makes the published policy false — revise this repo in the same change.

The support page also states which classes ship. Update it when that changes.

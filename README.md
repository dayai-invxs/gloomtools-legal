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

The policy claims the app collects nothing, contacts no server, and shares data
only peer-to-peer during party play. As of version 2.1 that is accurate:

- The app imports only Foundation, SwiftUI, Observation, and
  MultipeerConnectivity. There is no URLSession use and no third-party SDK.
- It writes `gloomtools.json` (characters) and `gloomtools-monsters.json` (the
  board) to its Documents directory, plus two UserDefaults keys: the party
  device identifier (`gloomtools.peerID`) and the dashboard zoom.
- Party play advertises the character name, party ID, and device identifier in
  the unencrypted Multipeer discovery info; the session itself uses
  `encryptionPreference: .required`. Guests persist the host's board; other
  players' characters are kept in memory only.
- The only permission is Local Network (`NSLocalNetworkUsageDescription`).

Any change to those facts — a new SDK, analytics, a crash reporter, cloud sync,
another permission, or a change to what a party shares or saves — makes the
published policy false. Revise this repo in the same change, and keep the app's
`PrivacyInfo.xcprivacy` in step.

The support page also states which classes ship and names on-screen buttons.
Update it when those change.

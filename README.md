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

The policy says the app collects nothing outside party play, and that party
play stores game state in Google Firebase under an anonymous sign-in. As of
version 2.2 (build 7) that is accurate:

- The app imports Foundation, SwiftUI, Observation, and from the Firebase iOS
  SDK only FirebaseCore, FirebaseAuth, and FirebaseFirestore. There is no
  Analytics, Crashlytics, Messaging, or other SDK, and no URLSession use.
- Solo play never touches Firebase. Sign-in happens only on Start, Join, or
  Rejoin (including the automatic rejoin at launch when a party code is saved).
- It writes `gloomtools.json` (characters) and `gloomtools-monsters.json` (the
  board) to its Documents directory, plus two UserDefaults keys: the saved
  party (`gloomtools.activeParty`) and the dashboard zoom. Firebase Auth keeps
  the anonymous user in the keychain; Firestore keeps a persistent cache.
- A party is `parties/{code}` with `members`, `state/board` and `characters`
  under it. Character documents are whole characters, including the name the
  player typed. Anyone signed in can join with the code; parties cannot be
  listed. Nothing is deleted by the app — leaving deletes only the member
  document. Every document carries `expireAt` (last write + 7 days), but no TTL
  policy is enabled: TTL needs billing, and the project stays on the free Spark
  plan. So the policy says party data is kept until deleted on request.
  Deleting a party means deleting `parties/{code}` **and** its `members`,
  `state` and `characters` subcollections — deleting the parent document alone
  leaves them.
- The app requests no permissions.
- `PrivacyInfo.xcprivacy` and the App Store Connect privacy label declare User
  ID and Gameplay Content: not linked, not tracking, App Functionality.

Any change to those facts — a new SDK, analytics, a crash reporter, another
permission, a change to what a party shares or how long it is kept, or turning
on TTL deletion (which the policy should then promise) — makes the published policy false. Revise this repo in
the same change, and keep the app's `PrivacyInfo.xcprivacy` in step.

The support page also states which classes ship and names on-screen buttons.
Update it when those change.

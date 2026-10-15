---
title: Privacy Policy
---

**GloomTools**

Effective date: October 15, 2026

## Contact

If you have questions about this policy, contact: consult.dayai@gmail.com

## Summary

GloomTools is a tool for playing Gloomhaven at the table. It has no accounts,
no sign-in, no analytics, and no advertising. Played on your own, it never
contacts the internet and nothing leaves your device.

If you start or join a party, the game state your party shares — your
character and the monster board — is stored in Google Firebase, a cloud
service, for the length of the party, so that every device at the table can
see it. Your device signs in to Firebase anonymously to do that. Nothing
in a party identifies you as a person, and we do not use party data for
anything except running the party.

## What we collect

Nothing outside party play. There is no analytics, no telemetry, no crash
reporting, and no advertising SDK in the app.

During party play, the party's data is stored in Firebase as described under
Party play below. We do not look at it, analyse it, or combine it with
anything else.

## What the app stores on your device

The app saves its data inside its own container so it is still there next time
you open it:

- **Your characters**: the names you type in, class, level, checked perks,
  manual deck edits, owned and equipped items, current health, conditions, the
  scenario's experience tally, the bless, curse, and scenario −1 cards in play,
  and the cards drawn so far this scenario
- **The monster board**: the monsters on it, their health and conditions, the
  monsters' deck and its recent draws, scenario level, and party size
- **A few settings**: the dashboard zoom level, and the code of the party you
  are in, so the app can rejoin it after a restart

This is app data, not an account. It never leaves the device except as
described under Party play and Backups below.

## Party play

Party play is optional. The app works fully without it, and nothing is sent
anywhere unless you start a party, join one, or rejoin one.

**How it connects.** Parties run through two Google Firebase services:
Firebase Authentication and Cloud Firestore. Every device in a party connects
to Firestore over the internet; the connection is encrypted. Google operates
these services on our behalf, under the
[Firebase privacy and security terms](https://firebase.google.com/support/privacy).
As with any internet service, Google receives your device's IP address when
the app connects.

**Anonymous sign-in.** When you first use party play, the app signs in to
Firebase anonymously. Firebase gives the device a random user identifier. It
is not linked to your name, email, phone number, Apple Account, or any
hardware or advertising identifier, and there is no password. It exists so the
party knows which device owns which character. Firebase keeps it in your
device's keychain.

**Party codes.** A party is identified by a six-character code shown on the
host's device. Anyone who has the code can join the party while it is
running, so share it only with the people at your table. Parties cannot be
listed or searched for; you can only join one whose code you have.

**What is stored in Firebase for a party.**

- Your character, in full: name, class, level, perks, deck, items, health,
  conditions, experience, and scenario cards. Other players see it on a shared
  dashboard.
- The monster board and the monsters' deck.
- The list of who is in the party, by character name (or "Display" for a
  device joined as a screen), with each device's anonymous identifier.
- The party code, which device started it, when, and whether it has ended.

**What other devices keep.** Every device in the party receives the party's
data, and Firestore keeps a local cache of it on each device so the party
keeps working through a brief loss of signal. Each device also saves the
current monster board in its own storage, replacing whatever board it had
before, so the scenario survives an app restart.

**When it stops.** Leaving the party, or the host ending the scenario, stops
your device sending and receiving party data.

## What the app does not do

- No accounts, sign-in, or password — the party sign-in is anonymous and
  automatic
- No advertising identifiers, and no tracking across other apps or websites
- No analytics or usage telemetry
- No location data
- No contacts, photos, camera, or microphone access
- No health data
- No push notifications
- No internet connections at all outside party play

The app asks for no permissions.

## Backups

If you have iCloud Backup or encrypted local backups turned on, iOS includes
the app's saved data in that backup, the same as it does for other apps. That
is handled entirely by Apple under
[Apple's Privacy Policy](https://www.apple.com/legal/privacy/), and we have no
access to it. Turning off backups for GloomTools in iOS Settings stops this.

## Sharing

We do not sell, rent, or trade your information. The only sharing is the
party play described above: with the other devices in your party, through
Google Firebase, and only when you choose to use it.

## Your choices

**Stop sharing.** Tap Leave Party on the Character tab.

**Clear the board.** On the Monsters tab, open the settings sheet and choose
Clear the Board.

**Delete a character.** Swipe a row on the Character tab and choose Delete. The
character and its deck are removed from your device immediately. A copy shared
in a party stays in Firebase until it is deleted on request, as described under
Data retention.

**Delete everything.** Delete the app from your device. iOS removes its
container, and with it every character, the board, and all settings. The
anonymous Firebase identifier may remain in the device keychain. It is not
linked to your identity.

**Ask us.** To have a party's data deleted from Firebase, email us with the
party code. We will delete everything stored for that party.

## Data retention

Data on your device lives there for as long as the app is installed, and is
gone when you delete the app.

Party data in Firebase is not deleted automatically. Ending a scenario closes
the party, so no one can join it and the app stops updating it, but its stored
data remains in Firebase until we delete it. We delete a party's data when
anyone in that party asks us to, and may delete old parties at any time.

A board you shared in a party also stays on the other party members' devices
until they clear it, end the scenario, or delete the app.

## Children

The app is not directed to children under 13, and we do not knowingly collect
personal information from children.

## Changes to this policy

If this policy changes materially we will update the effective date above and
publish the revision at this URL.

## Contact

Questions about this policy: consult.dayai@gmail.com

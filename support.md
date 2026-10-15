---
title: Support
---

# Support

**GloomTools**

For questions, bug reports, or feature requests, email consult.dayai@gmail.com.
We aim to respond within a few business days.

## The deck

### Why didn't the Shuffle button light up when I drew a bless?

Because no shuffle is owed. Only the deck's own ×0 and ×2 cards put the deck in
a shuffle-owed state. A bless is a ×2 and a curse is a ×0, but both leave the
game the moment they are drawn, so there is nothing to shuffle back in. A
scenario −1 is a plain −1 and never triggers one either.

### Why doesn't a rolling modifier draw the next card automatically?

By design. The card stays on the table so you can read it, the readout turns
orange and shows what the attack adds up to so far, and the Draw button changes
to **Draw Again**. Pressing it moves the rolling card into the history strip and
puts the next card down. The play area only ever holds one card.

### The app doesn't shuffle when I tell it a shuffle is owed.

That's deliberate. Gloomhaven shuffles at the *end of the round*, so the app
flags it — the Shuffle button turns orange — and leaves the timing to you.
Shuffling also clears the card on the table and the history, since a card left
on screen after a shuffle is a stale result.

### Where did my scenario −1 cards go?

They stay in the deck until the scenario ends. **End Scenario** in the scenario
sheet removes them along with any bless and curse cards.

## Scenarios, resting, and items

### What does End Scenario reset?

Health goes back to full, the experience tally is cleared, every item is
refreshed, and bless, curse, and scenario −1 cards are removed. The monster
board is cleared and the monsters' deck is reset. If you are in a party, the
party ends for everyone. Level, perks, and the items you own are kept.

### What does Long Rest do?

It heals 2, up to your maximum, and refreshes your *spent* items. *Consumed*
items stay consumed until End Scenario — that is the difference the game draws
between the two. Long Rest is never greyed out, even at full health with nothing
spent, because pressing it is how you mark that you rested. It can be undone.

### Why does my deck have extra −1 cards?

Some armour adds −1 cards to your deck while it is equipped. Those cards show
an ITEM chip in the deck editor and cannot be removed there; unequip the armour
on the Items tab instead. Classes with the perk that ignores negative item
effects do not get them once that perk is checked.

### Why don't monster conditions come off on their own?

The app does not know whose turn it is, so it does not referee. Take a token off
a standee in the app when you take it off the standee on the table. Bless and
curse are not in the conditions list because for monsters they are cards — add
them to the monsters' deck from the settings sheet on the Monsters tab.

## Party play and the TV dashboard

### How do we play as a party?

One player opens the Character tab and taps **Start a Party**; that player runs
the monsters. Their screen shows a six-character **party code** — read it out,
or use the share button beside it. Everyone else taps **Join a Party**, types
the code, and chooses to join as their character. Every device then shares its
own character and sees the same monster board.

Party play needs an internet connection on every device. The devices do not
need to be on the same Wi-Fi network.

Anyone with the code can join while the party is running, so share it only with
the people at your table.

### I can't join the party.

Check these, in order:

- **The code.** Codes are six letters and numbers, and never use 0, O, 1, I,
  or L, so there is nothing to mix up. It is on the host's Character tab, under
  Party.
- **An internet connection** on your device, and on the host's when the party
  was started.
- **The party is still running.** It ends when whoever is running the monsters
  ends the scenario, and a code cannot be reused after that.
- **Everyone has an up-to-date version** of the app.

### It says I'm offline.

Your device has lost its connection. Keep playing: your changes are kept and
sent as soon as the connection is back, and you catch up on everyone else's at
the same time.

### The app closed in the middle of a party.

Open it again. It rejoins the party you were in by itself. If it cannot reach
the party at that moment — usually for want of signal — a **Rejoin Party**
button appears on the Character tab.

### How do I put the party on a TV?

Use a spare iPad. On it, tap **Join a Party**, choose **Display**, and pick the
party. The iPad shows a dashboard with everyone's health and the whole monster
board, and keeps its screen awake. Connect it to the TV with an HDMI adapter or
AirPlay Screen Mirroring, and turn the iPad to landscape so the picture fills
the screen. The zoom buttons in the dashboard's header set the text size for
your room. A display edits nothing.

Chromecast is not supported.

### Someone's phone locked. Is their health out of date?

No. Nothing about a character changes while its owner isn't using their phone,
so the numbers everyone sees are still current.

### How do I hand the monsters to someone else?

If you are running the monsters, tap the people button on the Monsters tab and
pick who takes over. If you want them, tap **Take the Monsters** — they are
yours straight away, without waiting on the current owner, so agree it at the
table first.

### Why can't I end the scenario?

Only whoever is running the monsters can, because it ends the scenario for the
whole party.

### How do I leave a party?

Tap **Leave Party** on the Character tab. A display has a leave button in its
header.

## Characters

### How do I change who I'm playing as?

Tap anywhere on a character's row on the Character tab. To open a character's
setup instead — level, perks, deck editor — tap the gear on the right of their
row. Selecting and editing are separate on purpose, so you can check another
character's perks mid-scenario without losing your place. In a party, leave and
rejoin to play a different character.

### Does experience carry between scenarios?

No. GloomTools is a scenario toolkit, not a campaign tracker. Experience is a
per-scenario tally, and level is something you set by hand to match your
character sheet. There is no perk slot budget either — check the boxes your
character actually has.

### My class isn't in the list.

The current release covers sixteen of the seventeen Gloomhaven base-set
classes — the Quartermaster is not in yet, and neither are the Forgotten
Circles, Jaws of the Lion, or Frosthaven classes. In the
meantime you can build any deck by hand: pick the closest class, then use the
deck editor from a character's setup screen to add and remove cards.

### A perk looks wrong.

Please tell us, with the class and the perk. Perk lists are the part most worth
getting exactly right, and we would rather hear about it than have you play a
scenario with the wrong deck.

## Your data

### Is my data backed up anywhere?

Only in your device's own iOS backup, if you have that turned on. The app has
no accounts, so there is no cloud copy of your characters. Party play stores
the party's characters and board online so the devices at the table can share
them; email us with your party code if you want that copy deleted. It is not a
backup and does not carry characters between your own devices.
Deleting the app deletes everything on your device. See the
[Privacy Policy](privacy) for details.

---

[Privacy Policy](privacy) · [Home](./)

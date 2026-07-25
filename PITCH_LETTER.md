# A proposal for Grandpa Beck's Games

External, send-ready version of the pitch. Internal reasoning, open
questions, and personal notes live in `PITCH.md` — this file is the
version meant to actually reach Grandpa Beck's team, so keep it clean of
anything not meant for that audience.

---

Hi — I'm Parker. I built something I think you'll want to see: a free
companion app for the three Grandpa Beck's games that currently rely on
paper score pads — Skull King, Antiquity Quest, and Another Man's
Treasure.

One quick note up front: I'm not affiliated with Grandpa Beck's Games —
just a customer who likes these games enough to have built this on my own
time. Everything below is a genuine proposal, not a vendor sales pitch.

**Try it yourself:** https://parker-schwarz.github.io/skull-king-scorer/
No install, no account — open it on your phone and start a table.

## Two things this solves

**1. No one has to be the scorekeeper.** Right now, each of these games
ships with a printable score sheet, and every sheet has the same problem:
one person at the table has to fill in everyone's numbers by hand. This
app removes that job. Each player scores their own card, on their own
phone, and the app enforces the rules so the numbers come out right. It
also answers the question that comes up almost every round — *"wait,
who's winning?"* — instantly, for everyone, instead of someone doing table
math out loud.

**2. It's a real marketing touchpoint.** The winner screen after every
game reaches players at the exact moment they're happy — and can
introduce them to your other games. This isn't a guess: building this app
was the first time I personally realized how many games you actually
make. I'd bet a fair number of your customers are in the same boat, and
this is a natural way to close that gap.

## What it does

**One app, three games.** Swipe between Skull King, Antiquity Quest, and
Another Man's Treasure — each shown with its real box art on a backdrop
matched to its cover.

**Everyone keeps their own scorecard.** The host starts a table and gets
a 6-letter code. Everyone joins on their own phone, scores their own
card, and live standings show the whole table. It also works fully
offline as a solo scorepad.

**It handles the scoring paper can't:**
- *Skull King* — full bid/tricks/bonus scoring, plus a sanity check that
  the tricks entered add up to the round number
- *Antiquity Quest* — the full Beckston University Museum Logbook; the
  500-point explorer bonus computes itself, including the rulebook's
  twist where it passes to another qualified player if the first one out
  missed a collection type
- *Another Man's Treasure* — Classic and Progressive modes; used
  collection patterns grey themselves out automatically, enforcing
  once-per-game without anyone having to track it by hand

**It looks like one of your products.** Your badge logo, real box art,
your site's palette and typography, and how-to-play video links pulled
straight from the printed rulebooks.

## Built-in marketing, not bolted on

Every finished game ends on a branded winner screen with two things on
it:

1. Your own newsletter signup, recreated — name, email, a discount —
   captured at the exact moment the table is happy, tagged by which game
   was played. It's not wired to a real mailing list yet (that's a fast
   change whenever you're ready), and nothing is collected without a
   player choosing to opt in.
2. A "Shop All Grandpa Beck's Games" link into your full catalog — stays
   current as new games launch without ever touching the app.

Your own rulebooks already make this case: *"Out of score sheets? Print
or order more at GrandpaBecksGames.com."* This app is a more permanent
answer to that sentence — one that can email the customer back
afterward.

## One more thing — the Easter eggs

Double-tap the game title on any scorecard and each game's hidden persona
shows up:

- **Skull King — the Oracle.** Enter your hand and play order, and it
  recommends a bid with pirate commentary.
- **Antiquity Quest — Remington's Appraisal.** A professor character reads
  your actual scorepad and tells you what still matters for the bonus —
  with some snark.
- **Another Man's Treasure — Ask the Deer.** A groovy sunglasses deer
  suggests collection patterns you haven't used yet.
- **The GRANDPA crown.** Join a table as "Grandpa" and your name wears a
  bowler-hat crown everywhere it appears.

These aren't just jokes — they show the app doesn't just score the games,
it understands them well enough to advise mid-game in each one's own
voice.

## Built responsibly

- It's a single, simple web page on free hosting — running costs are
  effectively zero, no server to maintain
- Reviewed for common web security issues, with no sensitive data
  exposed and no secrets in the code
- No personal data is collected today — signups stay on-device until
  connected to a real mailing list, with your say-so

## Where this could go from here

If this is something worth exploring further, some natural next steps:

- Connect the email signups to your actual mailing list (a fast change)
- A QR code on physical score pads or box inserts pointing at the app —
  every box already sold becomes a distribution channel
- Deep links from the app into each game's real product page
- Anonymous play stats (games finished per week, most-played game) — a
  window into engagement you don't currently have once a box leaves the
  warehouse
- Swapping in real art assets from your design team in place of my site
  crops

I'd love to walk you through it, live or over a quick call — whatever's
easiest.

— Parker Schwarz
parkerschwarz@gmail.com

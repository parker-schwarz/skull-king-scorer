# Grandpa Beck's Scorepad — pitch notes

A free companion app for the three Grandpa Beck's games that use score pads:
Skull King, Antiquity Quest, and Another Man's Treasure. One link, no app
store, works on any phone. Open `scorepad.html` on any device to try it.

## The pitch in one line

Paper score pads get used up and thrown away. This one is permanent, does
math the pads can't, and ends every game night on a Grandpa Beck's branded
screen that grows the email list.

## What it does

**One app, three games.** Swipe between Skull King, Antiquity Quest, and
Another Man's Treasure — each shown with its real box art on a backdrop
matched to its cover (the plaid behind the AMT box is the box's own plaid).

**Everyone keeps their own scorecard.** The host starts a table and gets a
6-letter code. Everyone joins on their own phone, scores their own card, and
the live standings show the whole table. Works offline as a solo scorepad too.

**It enforces rules paper can't:**
- *Skull King* — bid/tricks/bonus scoring with every bonus type, plus a
  sanity check that the tricks entered add up to the round number
- *Antiquity Quest* — the full Beckston University Museum Logbook; the
  500-point explorer bonus computes itself, including the rulebook's twist
  where it passes to other qualified players if the first player out missed
  a collection type
- *Another Man's Treasure* — Classic and Progressive modes; used collection
  patterns grey themselves out with the round they were played, enforcing
  once-per-game automatically. Lowest wins, ties broken by patterns completed.

**It looks like a Grandpa Beck's product.** The badge logo in every header,
real box art, the site's palette and typography (Figtree, brick red, dark
teal, cream, gold), and how-to-play video links pulled from the printed
rulebooks.

## The marketing engine (why this is worth owning)

Every finished game ends on a branded winner screen with two things on it:

1. **The site's own newsletter popup, recreated** — "A gift from Grandpa,"
   name + email, 10% off. It captures at the exact moment the table is happy
   and laughing, and it drops into the same list the website already feeds
   (Klaviyo/Mailchimp/Shopify — currently a demo stub), tagged by which game
   was played. The website popup only catches people while shopping; this
   catches them right after they loved one of the games.
2. **A "Shop All Grandpa Beck's Games" link** into the full catalog — stays
   current as new games launch without ever touching the app.

And the rulebooks already make the case: "Out of score sheets? Print or
order more at GrandpaBecksGames.com." The app is the permanent answer to
that sentence — one that emails you the customer afterward.

## The Easter eggs (the demo closer)

Double-tap the game title on any scorecard and each game's hidden persona
appears:

- **Skull King — the Oracle.** Enter your hand and your play order in the
  first trick, and it recommends a bid with pirate commentary ("Going 2nd —
  ye see the table before ye play"). Position genuinely factors into the
  math.
- **Antiquity Quest — Remington's Appraisal.** Professor Remington reads
  your actual scorepad and tells you what matters: which collection types
  you still need for the 500-point bonus, character cards burning a hole in
  your hand, and your standing — with in-character snark ("My last assistant
  moved faster — and she went rogue.").
- **Another Man's Treasure — Ask the Deer.** The sunglasses deer dispenses
  groovy wisdom and only ever suggests collection patterns you haven't used
  yet.
- **The GRANDPA crown.** Join any table under the name "Grandpa" and your
  scorecard wears a bowler-hat crown everywhere your name appears. Have him
  join the demo table with his own name and let him find it.

The eggs make a bigger point: the app doesn't just score the games, it
*understands* them — deeply enough to advise mid-game in each game's own
voice.

## Built responsibly

- Single HTML file on free-tier hosting — running costs are effectively zero
- Security-hardened: pinned, integrity-checked dependencies; no secrets in
  the code; XSS and prototype-pollution guards; documented database rules
- No emails or personal data are collected in the demo — signups stay
  on-device until wired to the real list provider

## Easy next steps if he bites

- Email capture wired to his actual list provider (a one-day change)
- QR code on the physical score pads / box inserts pointing at the app —
  every box already sold becomes distribution
- Deep links to each game's real product page
- Anonymous play stats (games finished per week, most-played game) — market
  visibility he currently loses the moment a box leaves the warehouse
- Production art assets from his design team in place of the site crops

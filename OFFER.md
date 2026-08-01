# Grandpa Beck's Scorepad: Offer and Scope of Work

**Prepared for:** Grandpa Beck's Games
**Prepared by:** Parker Schwarz (parkerschwarz@gmail.com)
**Date:** [DATE]
**Offer valid through:** [DATE + 60 days]

Companion document to the pitch letter. The letter explains why this is
worth having. This one explains exactly what you'd be getting, what it
costs, who owns it afterward, and where my involvement ends.

**Live demo:** https://parker-schwarz.github.io/skull-king-scorer/

---

## The offer in one paragraph

I've already built a working companion scorepad app for Skull King,
Antiquity Quest, and Another Man's Treasure. It's finished, branded to
your site, and playable today. I'm offering to hand it to you outright:
the code, the app, and all rights to it become yours. Alongside that
transfer, I'll do the work of making it production-ready under your name
(wiring the newsletter capture to your real mailing list, swapping my
site crops for your actual art files, brand QA, live playtesting), write
the documentation, and support it for 90 days after launch while your
team or a contractor takes over. Total fee is **$9,000**, split across
three phases. After the 90 days, the app is entirely yours to run, and
I'm available hourly if you want me.

---

## Two things to be clear about up front

**The app stays free to players.** Nothing in this offer changes that. No
paywall, no in-app purchase, no ads. What's priced below is ownership of
the software and the work to make it something you can rely on, not
access for your customers.

**I built this independently, before any agreement existed.** I'm a
customer, not a vendor you've worked with. Everything in the app was
built on my own time using materials already public on your site. All
Grandpa Beck's trademarks, box art, game rules, and brand assets are and
remain yours. I claim no rights to any of them, and if you'd rather this
went no further, say the word and I'll take the demo down. This offer is
me asking whether you want it, not a bill for work you didn't order.

---

## What you'd be getting

A single-page web app, no install and no account, that works on any phone
with a browser.

**Three games in one app.** Skull King, Antiquity Quest, and Another
Man's Treasure (Classic and Progressive), each presented with its box art
on a matched backdrop.

**Each player scores their own card.** The host starts a table and gets a
six-letter code. Everyone joins on their own phone and scores themselves,
with live standings for the whole table. Nobody has to be the
scorekeeper. Players without a phone can be added as guests and scored by
the host. It also works offline as a solo scorepad.

**Scoring rules the printed sheets can't enforce:**

- Skull King: full bid, trick, and bonus scoring, with a check that the
  tricks entered add up to the round number
- Antiquity Quest: the full Beckston University Museum Logbook, with the
  500-point explorer bonus computed automatically, including the rulebook
  case where it passes to another qualified player
- Another Man's Treasure: used collection patterns grey themselves out
  automatically, so once-per-game is enforced without anyone tracking it
  by hand

**A post-game marketing screen.** Every finished game ends on a branded
winner screen carrying your newsletter signup (name, email, discount),
tagged by which game was played, plus a "Shop All Grandpa Beck's Games"
link into your catalog.

**Four Easter eggs.** Double-tapping a game title reveals a hidden
persona per game: the Oracle for Skull King, Remington's Appraisal for
Antiquity Quest, Ask the Deer for Another Man's Treasure, and a bowler-hat
crown for anyone who joins a table as "Grandpa."

**On-brand throughout.** Your badge logo, real box art, your site's
palette and typography (Figtree, brick red, dark teal, cream, gold), and
how-to-play video links pulled from the printed rulebooks.

---

## Scope of services

### Phase A: the app and the transfer

Everything described above, already built and working, transferred to
you. Concretely, that means:

- The repository moves into a GitHub organization you control, with full
  commit history
- The live URL moves to a domain or GitHub Pages site you own (a
  subdomain like `scorepad.grandpabecksgames.com` is straightforward if
  you want one)
- The Firebase project backing the live score sync is recreated under
  your account, so the running service is yours end to end
- All copyright and rights in the code transfer to you on final payment

I hand over admin. You don't inherit a dependency on my accounts.

### Phase B: production readiness

The work between "impressive demo" and "something you'd put your name
on."

- **Newsletter capture wired to your real list.** Today the signup form
  is a working demo that keeps entries on the device and sends them
  nowhere. I'll connect it to whatever you actually use (Klaviyo,
  Mailchimp, Shopify Email), tagged by game so you can see which title
  produced which signup.
- **Real art assets.** The box art and backdrops currently in the app are
  crops from your public website. I'll replace them with source files
  from your design team, at proper resolution.
- **Brand QA.** A side-by-side pass against your live site to get the
  teal and cream values exactly matching rather than approximately, and
  removal of an unused font import.
- **Product deep links.** The "Shop All Games" link becomes per-game
  links into the right product pages, so a table that just played Skull
  King sees Skull King.
- **A supervised pilot.** Real game nights on real phones across
  different networks, ideally including at least one player who has never
  seen the app, with fixes for whatever that surfaces. This is the step
  that matters most and the one nobody can skip.
- **Privacy and legal review support.** Once signups reach a real list,
  you have real obligations. I'll make sure the consent language, your
  privacy policy link, and the data flow are all wired correctly and
  documented for whoever reviews them.

### Phase C: documentation, handoff, and 90 days of support

- Written documentation covering how the app is structured, how to run it
  locally, how to deploy a change, how the Firebase side works, and where
  every game's scoring logic lives
- A walkthrough session with whoever will own it, your team or a
  contractor you hire, with a recording if useful
- **90 days of bug fixes from launch day.** If something breaks or scores
  wrong, I fix it, at no additional cost, within two business days for
  anything that stops a game from being played
- At the end of the 90 days, ownership of maintenance is fully yours

---

## Where my involvement ends

I want to be straight about this, because it's the part most likely to
cause a problem later if it's fuzzy now.

My background is accounting, not software. I built this because I like
these games and the problem was interesting. I'm not in a position to be
indefinite on-call support for a production tool your customers depend
on, and promising otherwise would be doing you a disservice.

So the offer is deliberately bounded. I build it, I harden it, I document
it, I fix what breaks for 90 days, and then it's yours. The app is
written specifically to make that handoff cheap: one HTML file, no build
pipeline, no framework to learn, no deployment system to inherit. Any
competent web developer can pick it up in an afternoon.

After the 90 days, three things can happen, and you can decide later:

1. You bring it in-house or hand it to a contractor. My preference, and
   what the codebase is built for.
2. You hire me hourly for specific changes, at $125/hour, no retainer and
   no minimum.
3. Nothing. It keeps running. A static file on free hosting doesn't rot,
   and there's no server to patch.

---

## What's not included

Naming these now so nobody is surprised later.

- Native iOS or Android apps. A scorepad used once a game night is better
  as a link than an install, and store presence would add developer
  accounts, review cycles, and a second codebase for no real gain. Happy
  to revisit if you want store presence for other reasons.
- Games beyond the three named here, including expansions. Priced
  separately below.
- Ongoing feature development past Phase B.
- Anything that isn't scoring. This is a scorepad, not a digital version
  of your games, not a play-online platform, and not an account system.
- Localization or translation.
- Your ESP subscription, domain registration, or any other third-party
  service fee.

---

## Optional add-ons

Priced separately. None of these are needed for launch.

| Add-on | Fee |
|---|---|
| A fourth game or expansion added to the app | $1,200 each |
| QR code artwork plus a print-ready score pad card or box insert | $600 |
| Anonymous play statistics (games finished per week, most-played game, average table size) with a simple dashboard | $1,500 |
| Custom subdomain setup and configuration | $250 |

The QR code one is worth a thought. Every box you've already sold becomes
a distribution channel the moment there's a code on the insert pointing
here.

---

## What it costs you to run

Effectively nothing, and I'd rather show the numbers than assert it.

The app is a single 287KB HTML file on GitHub Pages. React, Firebase, and
the other libraries load from public CDNs, and box art is served from
your own site, so each visit barely touches the hosting allowance.
GitHub's free tier covers 100GB of bandwidth a month, which works out to
roughly 350,000 page loads before it's even a conversation.

Live score syncing runs on Firebase's free tier: 1GB stored and 10GB
downloaded per month. A full game session moves a few hundred kilobytes
at most, so that's thousands of complete games a month before you'd need
to think about it.

If it somehow blew past both, the paid tier keeps the same free allowance
and then charges $5 per GB stored and $1 per GB downloaded. A genuine hit
lands in single-digit dollars per month.

There's no hosting bill worth budgeting for. The only real ongoing cost
is developer time when you want something changed.

---

## Pricing

| Phase | What it covers | Fee |
|---|---|---|
| A | The completed app, plus transfer of the code, the repository, the live service, and all rights | $5,000 |
| B | Production readiness: real mailing list integration, production art, brand QA, deep links, supervised pilot, privacy review support | $2,500 |
| C | Documentation, handoff walkthrough, and 90 days of bug fixes from launch | $1,500 |
| | **Total** | **$9,000** |

**Payment:** 50% on signing, 50% on completion of the Phase C handoff.

**Ownership transfers on final payment.** Until then I retain the
copyright, and you're free to walk away at any point before launch with
no further obligation beyond the deposit.

**Post-handoff work:** $125/hour, billed in 15-minute increments, no
retainer and no minimum commitment.

If you have a developer already and want to skip Phase B, or take on the
handoff work internally, those phases can be dropped and the fee comes
down accordingly. Say so and I'll re-cut the numbers.

---

## Timeline

Roughly four to six weeks from signing to launch, with the pilot being
the part that can't be rushed.

| Week | What happens |
|---|---|
| 1 | Repository and Firebase transfer, accounts set up, kickoff |
| 2 to 3 | Mailing list integration, production art swap, brand QA, deep links |
| 3 to 4 | Supervised pilot game nights, fixes from what they surface |
| 5 | Documentation and handoff walkthrough |
| 6 | Launch, then the 90-day support window begins |

Weeks 2 and 3 depend on how quickly I get the art files and mailing list
access, so that range moves with you, not with me.

---

## What I'd need from you

Short list, and none of it is heavy.

- Source art files for the three games (box art at print resolution, plus
  the badge logo)
- Access to your email platform, or an introduction to whoever
  administers it
- A GitHub organization to receive the repository, or someone to create
  one
- Product page URLs for the per-game shop links
- Two or three real game nights' worth of willing players for the pilot,
  ideally including someone who wasn't involved in building this
- One person named as the decision-maker, so questions don't stall

---

## Terms

- **Independent contractor.** This is a project engagement, not
  employment, and I carry my own taxes.
- **Confidentiality.** Anything you share (art files, list data, sales
  figures, product plans) stays confidential, indefinitely. Happy to sign
  your NDA.
- **Your IP stays yours.** Trademarks, box art, game rules, and brand
  assets are yours throughout and afterward. My rights are limited to the
  code I wrote, and those transfer to you on final payment.
- **Portfolio use.** I'd like to be able to say I built this and link to
  it. If you'd rather I didn't, that's fine, just tell me.
- **Either side can stop.** Before launch, either of us can end this with
  written notice. You pay for work completed to that point, and anything
  finished is yours.
- **This offer expires 60 days from the date above,** mostly so it
  doesn't sit in a drawer and turn into a misunderstanding a year from
  now. Ask and I'll extend it.

---

## Next step

Play a game on it first. Open the link on your phone, pull three or four
people in on theirs, and run a real hand of Skull King. Five minutes will
tell you more than this document will.

If it holds up, I'd like 30 minutes to walk through the rest and answer
whatever this doesn't.

**Parker Schwarz**
parkerschwarz@gmail.com
https://parker-schwarz.github.io/skull-king-scorer/

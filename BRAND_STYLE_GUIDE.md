# Grandpa Beck's Games — Brand Style Guide

Reference doc, not a one-off. Pulled from a live analysis of
grandpabecksgames.com so we stop re-deriving this every session. Update in
place if the site changes or a new subpage gets analyzed.

Last updated: 2026-07-25 (source: Claude Browser analysis of the homepage,
pasted in by Parker, cross-checked against six live screenshots)

## Screenshots

Six reviewed directly (hero, trust-badge strip, product grid, "Durable &
delightful" feature block, Instagram feed strip, footer) — details folded
into the sections below. They arrived as inline chat images, not files, so
the actual PNGs aren't committed to the repo. If we want them in
`/screenshots/brand/` for later reference, they need to be dropped in as
real files (drag into the project folder, or a download link) rather than
pasted into chat.

Note: the analysis text described a fifth "Play Together, Stay Together"
dark-teal testimonial section, but the fifth screenshot actually delivered
was the Instagram feed strip (`#GRANDPABECKSGAMES` grid) instead. The
testimonial section itself hasn't been screenshotted yet — worth grabbing
if it comes up again.

## Brand personality

Warm, nostalgic, family-first — a "gather around the table" feel, not a
slick corporate game brand. Leans into the "Grandpa" persona through
heritage cues (bowler-hat logo mark, hand-drawn flourishes) set against a
clean, modern e-commerce layout. Reads as trustworthy, wholesome, and
playful without being childish. Aimed at multi-generational families, not
just kids.

## Color palette

Warm and restrained, not a rainbow of game-box colors.

| Swatch | Hex | Use |
|---|---|---|
| Crimson / brick red | `#C92C2C` | Primary CTA buttons, announcement bar, accent lines |
| Deep teal-navy | `#08242B` | Footer, dark testimonial section |
| Teal-navy (lighter) | `#083744` | Footer/testimonial secondary |
| Mustard gold | `#C9930A` | Footer links, icons, decorative accents |
| Soft cream | `#F9EDBE` | Section background for badges/trust markers |
| Light neutral grey | `#F0EFEF` | Subtle section dividers |
| White | — | Dominant base background throughout |

Read: "vintage general-store meets modern DTC brand" — red/gold/cream evoke
old-fashioned playing-card and carnival aesthetics; dark teal grounds it so
it doesn't tip into full retro.

**How the app compares:** already close. `index.html` uses `#C92C2C`
(brick red) and `#C9930A` (gold) as exact matches, plus `#0D2B33`/`#123C47`
for teal (same family as the site's `#08242B`/`#083744`, slightly
different shade) and `#F5F1E6`/`#ECE5D3` for cream (same idea as the
site's `#F9EDBE`, not an exact hex match). Worth eyeballing side-by-side
once the screenshots land, but directionally on-brand already.

## Typography

Single font family for everything — **Figtree**, a rounded, friendly
sans-serif — used for both body copy and large hero headlines. No serif or
script font anywhere despite the "Grandpa" heritage branding; the
friendliness comes from color and illustration, not the typeface.

- Headlines: bold (weight 700), large (hero H1 ≈ 56px)
- Body: light, readable, 16px
- Buttons: slightly letter-spaced (1px), bold, all-caps styling — a
  "badge"/"stamp" feel matching the game-box aesthetic

**How the app compares:** matches — `index.html` uses Figtree as
`--f-title`/`--f-ui` throughout. One inconsistency: the app also imports
**Fraunces** (a serif) in the Google Fonts link but never actually applies
it anywhere in the CSS — dead weight worth dropping, and notably the site
itself confirms the "no serif" choice is deliberate, so this isn't a case
of the app innovating on-brand.

## Layout & page structure

Standard, well-executed DTC pattern, top to bottom:

1. Thin promotional announcement bar
2. Simple nav — logo left, utility icons (cart, account) right
3. Full-bleed lifestyle-photo hero, bold headline, single CTA
4. Three-column trust-badge strip (units sold, star ratings, "new
   experience" messaging), framed with gold scrollwork corners
5. Product grid (3 columns) — box art, one-line pitch, price
6. Alternating image/text feature blocks (image left/right, text
   opposite) making durability/design claims, separated by thin gold
   horizontal rules
7. "About the family" section with a group photo
8. Dark-background testimonial section with quote-bubble icons
9. Instagram feed strip
10. Dark-teal footer — three link columns, payment-method icons

## Confirmed from screenshots — exact copy & structure

**Announcement bar:** "Free Shipping over $50" — white text on brick red.

**Nav:** logo left (bowler-hat mark + "GRANDPA BECK'S GAMES" wordmark,
black on white) — How-to-Play, Retailers, Printables, Gear — red "SHOP
GAMES" button, cart icon, account icon, right-aligned.

**Hero:** full-bleed family photo. Headline "Deal a Handful of Fun" (white,
bold, large). Subhead "We make great games so you can make great
memories." Single red "SHOP GAMES" CTA, centered.

**Trust-badge strip** (cream bg, gold corner scrollwork, thin gold rule
below), three columns, each an illustrated icon + italic teal headline +
red all-caps micro-label:
- Ribbon icon — "Over three million games sold" / "OUR #1 BEST SELLER"
- Stars icon — "Tens of thousands of 5-star reviews" / "WHAT PEOPLE ARE
  SAYING"
- Cards icon — "A new experience with every shuffle" / "THE GRANDPA
  BECK'S DIFFERENCE"

**Product grid section:** headline "Game time is time well spent",
subhead "We make games that bring pure enjoyment to everyone." Cards
observed: The Ticket Booth ($19.99), Cover Your Assets® ("Addictive game
of give and take. Loved by all ages!", $19.99), Skull King® ("The
Ultimate Pirate Trick Taking Game", $19.99), plus Whoa There Cowboy and
3-2-1 Countdown partially visible below the fold.

**"Durable & delightful" feature block:** bold teal headline, two short
body paragraphs ("Say hello to attractive designs, durable cards, and
sturdy boxes." / "We use premium materials to make our games sturdy for
lots of shuffling and travel bumps. Plus, our detailed artwork will
delight players of all ages."), red "SHOP GAMES" button, image of
scattered Skull King cards opposite the text, thin gold rules above and
below.

**Instagram feed strip:** tiled grid of mixed content — product lifestyle
shots, in-app-style card graphics, a travel/event photo ("Come with us to
Origins!"), tagged `#grandpabecksgames` implicitly via the footer social
handle.

**Footer** (dark teal-navy bg, gold link text): three columns —
- MENU: Retailers, Blog, Games, FAQ, Contact, Customer Service, Media
  Room, Affiliate Program
- RULES AND THINGS: Scorepads, Coloring Pages, JK Studios
- #GRANDPABECKSGAMES: Facebook, Twitter, Pinterest, Instagram, YouTube

Below that: copyright line, "Powered by Shopify," a row of payment-method
icons (Amex, Apple Pay, Diners, Discover, Google Pay, Mastercard, PayPal,
Shop Pay, Visa), and a legal-links row (Privacy Policy, Cookie Policy,
Acceptable Use Policy, Terms of Service, Returns page).

**Persistent lead-capture popup:** small "Get 10% Off" tab, bottom-left
corner, dismissible with an X — present across every page, not just the
homepage. Worth noting since the app's own post-game newsletter capture
is a different UI pattern (full-screen branded moment vs. this site's
low-key persistent corner tab) — that's a deliberate app improvement, not
a mismatch to fix.

**Note:** "Scorepads" appears as its own footer link under "Rules and
Things" — meaning the site already sends traffic to a scorepad-related
page. Worth checking that page before the pitch; it may be exactly where
an app like this would get linked from.

## Imagery style

- Photography: real, candid-looking multi-generational families genuinely
  engaged in play — not posed stock-photo smiles
- Product photography: straightforward box-art shots on white/neutral
  backgrounds
- Illustration accents (trust badges, corner flourishes): hand-drawn,
  engraved/vintage-badge style in the gold/teal/red palette — not flat
  modern icons

## Voice & messaging tone

Short, warm, benefit-driven — connection and memory-making over feature
lists. Section headers are punchy and conversational, not corporate
("Grandpa Beck and his crew," "Play Together, Stay Together"). Product
descriptions run one or two sentences, emphasizing the feeling of play
over rules/mechanics. Trust-building leans on social proof (units sold,
star-review counts) over technical claims.

## Recurring UI/component patterns

- Persistent shipping-threshold announcement bar
- Red rectangular buttons, thin matching border, generous horizontal
  padding
- Gold decorative corner scrollwork bookending sections
- Thin gold horizontal divider rules between sections
- Red "SHOP GAMES" CTAs repeated every 2–3 scroll sections — conversion
  paths stay present without feeling pushy

## The scorepads page — direct pitch evidence

`https://www.grandpabecksgames.com/pages/scorepads` — confirmed via
screenshots. This is the single strongest piece of evidence for the
pitch: the site's current answer to "how do I score this game" is a
downloadable PDF you print and fill in by hand.

**Page structure:** one section per game, each showing the relevant box
art thumbnail(s) with a red "Score Sheets" link underneath that downloads
a printable PDF.

- **Antiquity Quest** — base game + expansion box art, each with its own
  "Score Sheets" link
- **Skull King** — base game + Legendary Expansion box art, each with its
  own "Score Sheets" link
- **Another Man's Treasure** — two separate downloads: "Classic Game
  Score Sheet" and "Progressive Game Score Sheet"

So at minimum 4+ distinct PDFs live behind this one page.

**What the sheets actually require of the player** (this is the pitch):

- *Antiquity Quest sheet* — a grid with First/Second/Third Round rows,
  each split into Bonus Points / Collection Points / Card Points / Round
  Score, plus a Grand Total row. A footnote instructs the player to
  "consult rule book for complete scoring instructions" for the 500-point
  bonus — i.e., the sheet doesn't compute anything, it just holds numbers
  the player calculated by hand. The app already automates this bonus,
  including the pass-along rule.
- *Skull King pad* — a themed but still fully manual grid: numbered rows
  1–10 (rounds) with blank cells per player, no bid/trick math done for
  you.
- *AMT "Classic Game Patterns" sheet* — the clearest example. It's a
  printed lookup table of the 5 scoring patterns and their point values
  ("2 Sets of 4," "2 Suited Runs of 4," "1 Suited Run of 4 + 1 Set of 4,"
  "1 Suited Run of 8," "4 Suited Pairs"), repeated 4× on one page so it
  can be cut into 4 separate score cards, plus a handwritten-style
  footnote explaining the suited-color-matching rule. The player has to
  manually track which patterns they've already used. The app's
  "used patterns grey themselves out" feature replaces this table and the
  manual tracking entirely.

**Pitch framing this supports directly:** the app isn't competing with an
imagined future product — it's replacing a process that already visibly
frustrates the company enough that they built and host printable
replacement sheets. "Out of score sheets? Print more" (per `PITCH.md`) is
literally this page.

**The sharper version of the pitch (Parker's framing, more precise than
"does math paper can't"):** every one of these PDFs still has the same
structural bottleneck — one person at the table has to be the
scorekeeper, filling in everyone's numbers by hand on a single sheet.
The app's actual advantage isn't just automated math, it's that the
bottleneck disappears: each player scores their own card, on their own
phone, live, with no single person responsible for the group's sheet.
That's the "options and convenience" pitch. And because scoring now
happens through the app instead of a pencil, the moment the game ends is
also a marketing moment — the newsletter capture screen — which a paper
sheet structurally cannot offer. Lead with *distributed scoring +
convenience*, with *automated math* and *the marketing touchpoint* as
supporting points underneath it, not the headline.

## Open follow-ups

- [x] Six screenshots reviewed (hero, trust badges, product grid, feature
      block, Instagram strip, footer) — details captured above. Decision:
      not committing the actual image files to the repo; the written
      detail is what's actually useful for building/comparing against
- [ ] Grab the "Play Together, Stay Together" dark-teal testimonial
      section specifically — described in the original analysis but never
      actually screenshotted (low priority, not blocking)
- [x] Document `/pages/scorepads` — confirmed via screenshots, see
      section above; sharpened the core pitch angle to "distributed
      scoring removes the single-scorekeeper bottleneck," not just
      "automated math"
- [ ] Side-by-side check of app teal/cream hex values against the site
- [ ] Consider checking a subpage (product page template, blog) for
      additional style notes
- [ ] Decide whether to drop the unused Fraunces font import from
      `index.html`

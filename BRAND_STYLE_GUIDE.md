# Grandpa Beck's Games — Brand Style Guide

Reference doc, not a one-off. Pulled from a live analysis of
grandpabecksgames.com so we stop re-deriving this every session. Update in
place if the site changes or a new subpage gets analyzed.

Last updated: 2026-07-25 (source: Claude Browser analysis of the homepage,
pasted in by Parker)

## Screenshots

Pending — six to be added: hero section, trust-badge strip, product grid,
"durable and delightful" feature block, "Play Together, Stay Together"
section, footer. Drop them in `/screenshots/brand/` and link here once
available.

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

## Open follow-ups

- [ ] Add the six screenshots (hero, trust badges, product grid, feature
      block, "Play Together" section, footer)
- [ ] Side-by-side check of app teal/cream hex values against the site
      once screenshots are in
- [ ] Consider checking a subpage (product page template, blog) for
      additional style notes
- [ ] Decide whether to drop the unused Fraunces font import from
      `index.html`

# Progress — Grandpa Beck's Scorepad

Living status doc. Update this as things change; don't let it go stale.
Pairs with `PITCH.md` (internal pitch reasoning), `PITCH_LETTER.md`
(the send-ready version addressed to Grandpa Beck's team), and
`BRAND_STYLE_GUIDE.md` (their site's palette/type/voice, for keeping
anything client-facing on-brand) — this file is the honest internal read
on where things actually stand.

Last updated: 2026-07-25

## Where it lives

**Live:** https://parker-schwarz.github.io/skull-king-scorer/
Static single-file app (`index.html`) on GitHub Pages, syncing live scores
through a shared Firebase Realtime Database project. No build step, no
server to run, no hosting bill — free tier covers this comfortably.

## What's built (feature-complete as of the last commit, Jul 19 2026)

- All three games playable end to end: Skull King, Antiquity Quest,
  Another Man's Treasure (Classic + Progressive)
- Host/join flow with 6-letter table codes; each player scores their own
  card; live standings sync across devices; guest players without a phone
  can be added and scored by the host
- Game-specific rules enforcement (bid/trick sanity check, Antiquity
  Quest's 500-pt explorer bonus incl. pass-along rule, AMT once-per-game
  pattern greying)
- Branded throughout: real box art, badge logo, site palette/typography
- Post-game marketing screen: newsletter capture + "Shop All Games" link
- Easter eggs: the Oracle, Remington's Appraisal, Ask the Deer, the
  GRANDPA crown
- Security-hardened: pinned/integrity-checked deps, XSS/prototype-pollution
  guards, no secrets in the code

See `PITCH.md` for the full sell. See commit history for the build order.

## Pitch materials — now genuinely send-ready

- `BRAND_STYLE_GUIDE.md` — Grandpa Beck's actual site palette, type
  (Figtree), layout rhythm, voice, and confirmed page structure
  (including `/pages/scorepads`, their existing printable-PDF score
  sheets — direct evidence for the pitch). Sourced from a live site
  analysis plus screenshots, cross-checked against `index.html`'s CSS
  (already close to on-brand; one unused Fraunces font import flagged
  for cleanup).
- **Sharper pitch angle**, now the lead in both pitch docs: the real
  problem paper score sheets create isn't missing math, it's that one
  person has to be the scorekeeper. The app's headline value is
  distributed self-scoring + instant "who's winning" standings;
  automated math and the marketing touchpoint are supporting points.
- `PITCH_LETTER.md` — a second, client-facing version of the pitch,
  separate from `PITCH.md`. Addressed directly to Grandpa Beck's team in
  second person, discloses up front that this is an unaffiliated
  customer proposal, leads with a "try the live demo" link, and closes
  with contact info instead of internal next-step notes. `PITCH.md`
  stays the internal-reasoning version — open questions, personal notes,
  "if he bites" framing — and should never be the one actually sent.
- Both pitch docs have styled HTML previews (Claude Artifacts, private
  until shared) matching Grandpa Beck's brand palette for an easy
  read-through before sending anything for real.

## What's NOT done / not true yet

- **No real game has been played on it.** Everything above is
  feature-complete but untested under actual game-night conditions —
  multiple real phones, real Wi-Fi/cell flakiness, a non-technical player
  (ideally an actual grandparent) using it cold.
- **Newsletter capture is a demo stub.** Signups stay on-device; not wired
  to a real ESP (Klaviyo/Mailchimp/Shopify). Noted honestly in `PITCH.md`.
- **No production art assets** — box art/backdrops are crops from the
  public site, not source files from Grandpa Beck's design team.
- **No QR code / deep link into the app from a physical product** yet.

## Open decision: native app vs. web link

**Resolved for now: web link only, not a native app.** Reasoning: a
native app adds real ongoing cost and complexity (developer accounts, app
review, a wrapper toolchain or a second codebase) for a use case — a
score pad used once per game night — where a link or QR code is actually
*less* friction than an install. It also converts "who maintains this" from
a manageable question into a hard dependency on ongoing native dev work.
Revisit only if Grandpa Beck's team specifically wants store presence for
reasons beyond scoring (e.g. cross-promotion with other apps they own).

## Open question: who maintains this after the pitch

This is the real blocker right now, not the app itself. Hosting and
uptime are close to solved by the architecture (static file + Firebase
free tier), but ongoing bug fixes / feature requests are a genuine open
question — Parker's background is accounting, not dev/ops, and isn't
signing up to be indefinite on-call support for a production tool.
Options to raise with Grandpa Beck's team rather than resolve solo:
- Parker maintains it informally as long as it stays small/low-traffic
- Grandpa Beck's company brings in a contractor to own it if/when it's
  proven — the codebase is intentionally simple (one HTML file, no build
  pipeline) specifically so that handoff is cheap
- Scope is capped explicitly at "scorepad," not open-ended feature requests

## Path to pitch-ready

- [x] Write the actual pitch materials (`PITCH.md`, `PITCH_LETTER.md`,
      `BRAND_STYLE_GUIDE.md`) — done and on-brand
- [ ] Run a full real game night on it (this is the next concrete step)
- [ ] Fix whatever the real game night surfaces
- [ ] Decide + write down the maintenance-ownership answer above before
      the pitch conversation, even if the answer is "let's figure it out
      together"
- [ ] (Optional, not blocking) Wire newsletter capture to a real ESP if
      there's time — otherwise pitch it as "one-day change" per
      `PITCH_LETTER.md`
- [ ] Final read-through of `PITCH_LETTER.md` before sending — check tone,
      length, and the "not affiliated" disclosure line
- [ ] Schedule time with Grandpa Beck / send `PITCH_LETTER.md`

## Bottom line

The app itself is in good shape — feature work is essentially done, and
the pitch materials are now genuinely send-ready. The gap between now and
pitching isn't more building or writing, it's (1) proving the app
survives a real game night and (2) walking in with a straight answer on
who owns this thing after the demo lands well.

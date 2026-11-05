# Lighthouse Keeper — Store Submission Materials

## Short description (CrazyGames / GameDistribution / itch.io)

Swing the lighthouse beam across a night sea. Reefs hide until your light
holds on them — relay the beam between ships, split it with prisms, boost it
with lenses, and bring every hull home through the fog.

(198 characters)

## Details

- Genre: Puzzle / Strategy / Timing
- Controls: Mouse / Touch (drag the sea to swing the beam in 15° steps, drag
  prism & lens tokens onto dashed slots). Keyboard: ←/→ rotate, R retry, M mute.
- Features: 25 handcrafted levels with verified solutions, prism beam
  splitting (±45°), lens range/intensity boost, fog attenuation, reef reveal
  windows on a 3-second beat clock, ship hull damage and dodging, score for
  beats left + hull saved, per-level best scores, procedural graphics and
  sound, single-file HTML5 (no external assets), works offline once loaded.
- Objective: every reef must be revealed before a ship crosses it. A ship
  that hits a dark reef sinks and the night is lost; revealed reefs are
  dodged, but narrow ones scrape 1 of 2 hull points.
- Scoring: remaining beats ×10 + remaining hull ×2. Best score per level is
  stored locally.
- Tech: Vanilla JavaScript, Canvas 2D, WebAudio. No frameworks, no tracking,
  no external links inside gameplay.

## Tags

puzzle, lighthouse, light-beam, logic, timing, ships, sea, single-file, casual

## CrazyGames submission checklist
- [x] Self-contained index.html (SDK loads only on crazygames domains)
- [x] gameplayStart / gameplayStop / happytime events wired (domain-guarded)
- [x] Responsive (canvas scales, landscape 520×424, touch-friendly)
- [x] No external links inside gameplay, no analytics
- [ ] Cover image (to be captured from live game, 1280×720)

## GameDistribution
- Upload `lighthouse-keeper-gd.zip` (contains only index.html).
- The GD SDK loader activates automatically on gamedistribution.com /
  gd.games hosts; no other changes needed.

## itch.io
- Upload `lighthouse-keeper-itch.zip`, mark "This file is playable in
  browser", entry file: index.html, viewport 520×424, kind: html.
- Pricing: $0 (donations optional)

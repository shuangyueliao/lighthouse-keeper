# Lighthouse Keeper

A free, original light-beam harbor puzzle. Single-file HTML5 — no external
assets, no tracking, no ads.

You are the night keeper of a lighthouse. Ships run fixed lanes toward your
port while unmarked reefs wait just under the surface. Swing the lighthouse
beam (15° steps), reveal each reef with sustained light before a ship sails
over it, and relay the beam between danger zones on a 3-second beat clock.

## Mechanics

- **Beam** — drag the sea (or ←/→) to swing the lighthouse light. Reefs only
  become visible after ~1s of sustained light and stay revealed for a short
  window, so the beam has to be relayed on schedule.
- **Prism** — splits the beam into two beams at ±45°.
- **Lens** — boosts intensity: bigger reveal radius and longer reach.
- **Fog** — dims the beam inside the bank (weak reveals only).
- **Ships** — 1–3 per night, fixed lanes, 2 hull points. Revealed reefs are
  dodged (narrow reefs scrape 1 hull); dark reefs sink the ship and end the run.
- **Scoring** — beats left ×10 + remaining hull ×2. Best score per level is
  saved locally.

25 handcrafted nights, from a single straight lane to prisms, lenses, fog and
three-ship relay schedules. Every level ships with a verified reference
solution timeline.

## Controls

- Mouse / touch: drag the sea to aim, drag device tokens onto dashed slots.
- Keyboard: ←/→ rotate 15°, R retry, M mute.

## Tech

- One `index.html` (~46 KB), vanilla JS, Canvas 2D, WebAudio (all graphics and
  sounds are procedural — no images, fonts or audio files).
- Portal SDK loader is domain-guarded: the CrazyGames SDK loads only on
  crazygames domains, the GameDistribution SDK only on gamedistribution /
  gd.games domains, nothing anywhere else. gameplayStart / gameplayStop /
  happytime are wired behind the same guard.
- Progress and mute preference are stored in localStorage (fully optional;
  the game runs fine with storage blocked).

## Run

Serve the file over HTTP (or open directly) — everything is inline:

```
python3 -m http.server 8000
# http://localhost:8000/
```

## License

MIT. All names, mechanics, art and audio are original creations for this
project; no third-party IP is used.

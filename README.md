# Coin Temple: Galactic

Retro Flower of Life shooter with upgrades, sponsor ships and a leaderboard. No build step, no dependencies.

## Files
- `index.html`: page shell
- `style.css`: styles
- `game.js`: game logic. Edit the `CFG` block at the top to set sponsor name, tagline, link and bonus, and an optional `endpoint` for a shared leaderboard.

## Run locally
Open `index.html` in a browser.

## WordPress
Upload the folder to your host and embed with an iframe, or paste the contents of `style.css` (in a style tag) and `game.js` (in a script tag) with the body markup into a Custom HTML block.

## Analytics events
Listen for `coin-temple` events on `window` (or `postMessage` on the parent page): `game_start`, `wave_clear`, `game_over`, `sponsor_impression`, `sponsor_click`.

## Deploy on Render (static site)
1. Push this folder to a GitHub repo.
2. On Render: New + > Static Site, connect the repo.
3. Build command: leave blank (or `echo static`). Publish directory: `.`
4. Deploy. (Or use New + > Blueprint, which reads `render.yaml`.)

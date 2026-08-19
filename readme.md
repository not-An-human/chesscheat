## Updates Of this fork 

## Not vibe coded but still AI was used for bundling the WASM part and CSS

Rewrite for Firefox with a local Stockfish engine instead of chess.com’s.

- **Bundled Stockfish WASM** (ASM.js fallback) — no longer uses chess.com’s worker
- **Dynamic red squares** — highlights update during search when a better move is found
- **Multiple lines**  — switch with the on-page panel, Tab / Shift+Tab, or keys 1–5
- **Keeps analyzing after each move** — new positions are queued instead of stalling the engine
- **Popup controls** — Start / Stop, depth, and number of lines (no injected page button so less detectable)

### Install (Firefox)

1. Open `about:debugging#/runtime/this-firefox`
2. Click **Load Temporary Add-on**
3. Select `manifest.json`

Then open a chess.com game and click **Start** in the extension popup.

---

## Use

1. Open a chess.com game
2. Click the extension icon → **Start**
3. Red squares show the active engine line
4. Switch lines with the panel, Tab / Shift+Tab, or keys 1–5

## Layout

- `scripts/background.js` — Stockfish worker and search queue
- `scripts/content.js` — board FEN, highlights, line panel
- `popup/` — start/stop, depth, MultiPV
- `engines/` — Stockfish WASM, ASM.js fallback



<p>Chess cheat utilizes the stockfish engine and the power of your computer to show you the best move to make in any chess.com game. It guarantees you wins in atleast 90% of games you play and can greatly help you improve your chess skills.

<i>Note: this project was developed for learning purposes, I do not condone or encourage cheating in games and this project should help you get better at chess. Non fair play might result in your chess.com account being suspended if you do not use wisely. </i>
<br>


https://user-images.githubusercontent.com/71329328/221189107-244544b0-8070-4ee3-973f-c4c9bfa15067.mp4

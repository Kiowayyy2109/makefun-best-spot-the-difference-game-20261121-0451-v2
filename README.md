# Harbor Lights — Spot the Difference

[![make.fun](https://make.fun/badge/best-spot-the-difference-game-20261121-0451.svg)](https://make.fun/bounty/best-spot-the-difference-game-20261121-0451)
[![rank](https://make.fun/badge/best-spot-the-difference-game-20261121-0451/Kiowayyy2109/makefun-best-spot-the-difference-game-20261121-0451-v2/rank.svg)](https://make.fun/bounty/best-spot-the-difference-game-20261121-0451)
[![reward](https://make.fun/badge/best-spot-the-difference-game-20261121-0451/Kiowayyy2109/makefun-best-spot-the-difference-game-20261121-0451-v2/reward.svg)](https://make.fun/bounty/best-spot-the-difference-game-20261121-0451)

**Harbor Lights** is an original spot-the-difference game: two near-identical
pictures side by side, seven hidden differences per scene, and a race against
the clock. Three hand-drawn (procedurally painted, Canvas 2D) scenes — a harbor
at dusk, a night market, and a mountain cabin in the snow — each with 7 real
differences: objects that appear or vanish, colors that change, counts that
shift, and things that move.

Click a difference on **either** picture to find it. Found differences get a
gold ring on both panels. Wrong clicks flash a red X and cost points and time.
Stuck? Spend one of your 3 hints per round (H) to briefly highlight an
unfound difference. Beat the 150-second timer, clear all three scenes, and
chase the best total score with accuracy and time bonuses.

## How to play

- **Mouse:** click a difference on either picture.
- **H** — hint (3 per round) · **R** — restart · **M** — mute · **1 / 2 / 3** — pick a scene from the menu.
- Score: +100 per difference, +time bonus on a cleared round, −10 per wrong click.
- Sounds are synthesized live with WebAudio — no audio files, no network.

## Run it

Serve the `game/` folder with any static server and open `game/index.html`
in desktop Chrome:

```sh
cd game
python3 -m http.server 8080
# open http://localhost:8080
```

Everything is offline: no network requests, no external assets, no fonts
beyond the system stack.

## Entry

Built for the make.fun competition
[best-spot-the-difference-game-20261121-0451](https://make.fun/bounty/best-spot-the-difference-game-20261121-0451).
`main.ts` hands the game in: it copies `game/` and `screenshots/` to the
output directory and writes `dossier.json` with the vendored
`vendor/makefun-game.ts` library.

---

Made with [make.fun](https://make.fun/?ref=8b9bbsfs) — build agents, enter competitions, get ranked in the open.

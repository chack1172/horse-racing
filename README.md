# 🏇 Corsa dei Cavalli

A chaotic browser horse race for nine players: nine random horses, one winner.
Archers, falling bombs, banana peels and turbo farts keep every race unpredictable.

The UI and live commentary are in Italian.

## Features

- Nine horses with random names, coats and silks
- Live leaderboard, total wins and top-5 best times (kept for the session)
- Random events: arrow volleys, bomb rain, banana slips, fart boosts
- Synthesized sound effects (Web Audio API) with mute toggle
- Spoken Italian commentary (Web Speech API, when an Italian voice is available)
- Light/dark theme following the system preference; respects `prefers-reduced-motion`

## Play

No build, no dependencies — it's a single HTML file.

- Open `index.html` in a modern browser, or
- Serve it locally with one of:
  - `npx serve .`
  - `python -m http.server 8000`
  - `php -S localhost:8000`

## Configuration

Tweak the constants at the top of the `<script>` in `index.html`:

| Constant | Purpose                                         |
| -------- | ----------------------------------------------- |
| `SPEED`  | Race pace (lower = longer race, default ≈ 25 s) |
| `HORSES` | Horses per race (default 9, max `NAMES` length) |
| `NAMES`  | Pool of horse names (`HORSES` drawn each race)  |
| `EVENTS` | Odds, timing and limits of the random events    |
| `COLORS` | Jockey silk colors, one per lane                |

## License

[MIT](LICENSE)

# Retro Neon Snake Odyssey

A browser-based Snake game with a retro cyberpunk aesthetic. Built as a single HTML file — no build step required.

**Play online:** [https://52110230608.github.io/snake/](https://52110230608.github.io/snake/)

**Repository:** [https://github.com/52110230608/snake](https://github.com/52110230608/snake)

## Features

- **Three game modes**
  - **Classic** — hitting a wall ends the run
  - **Portal** — wrap around screen edges
  - **Labyrinth** — procedurally generated walls each run
- **Solo or VS CPU** — race an AI rival on the same board (Easy → Ultra)
- **Solo pace** — Relaxed, Standard, or Aggressive (saved in browser)
- **Combo streaks** — eat coins within 2.5s for bonus points (up to 2×)
- **Power-ups (Nanites)**
  - Ghost — pass through your own body
  - Freeze — slow movement for tighter control
  - Multiplier — double points for a limited time
  - Shrink — instantly trim up to 3 tail segments
- **Four snake palettes** — Emerald, Cyber, Gold, Ocean
- **High score** — persisted locally in solo mode
- **Synthesized audio** — toggle sound on/off
- **Mobile support** — touch D-pad and swipe on the canvas

## Controls

| Input | Action |
|-------|--------|
| `W` `A` `S` `D` or Arrow keys | Move |
| `P` or `Esc` | Pause / resume |
| `Space` or `Enter` | Start / restart (from menu or game over) |
| Swipe on canvas | Move (touch devices) |
| On-screen D-pad | Move (touch devices) |

## Run locally

From the project folder:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.

You can also open `index.html` directly, but a local server is recommended.

**Requirements:** A modern browser and internet access (Tailwind CSS and Google Fonts load from CDNs).

## Project structure

```
snake/
├── index.html   # Game (HTML, CSS, and JavaScript)
├── README.md
└── .gitignore
```

## Tech

- HTML5 Canvas
- [Tailwind CSS](https://tailwindcss.com/) (CDN)
- [Google Fonts](https://fonts.google.com/) — Orbitron, Share Tech Mono
- Web Audio API for sound effects
- `localStorage` for high score and pace preference

## License

This project is provided as-is for personal use and learning.

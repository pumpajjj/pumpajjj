# PUMPAJJJ!

**Pumpajjj i podrži studentske blokade!**

A tiny browser toy in support of the student blockades in Serbia. Grab the bicycle pump, pump up the balloons, and pop them.

### ▶ [Play the demo](https://pumpajjj.github.io/pumpajjj/)

[![PUMPAJJJ! preview](preview.png)](https://pumpajjj.github.io/pumpajjj/)

## How to play

1. Drag the pump handle **down** to push air into the balloon on the valve.
2. Keep pumping until the balloon is full. It detaches and floats away.
3. Click or tap a floating balloon to **pop** it.
4. Every 5 balloons, the progress bar at the top fills up and you get a **PUMPAJ!** bonus.

Works with mouse and touch (pointer events), on desktop and mobile.

## Support the students

The graduation cap button in the corner and the banner link to [blokadnedonacije.rs](https://blokadnedonacije.rs/), where you can donate to support the students.

## Tech

No frameworks, no build step. Everything lives in a single `index.html`:

- The pump is an inline SVG (drawn in Inkscape).
- Balloon physics, tweens and the game loop are plain JavaScript with `requestAnimationFrame`.
- Sound effects use `<audio>` elements and the Web Audio API.

## Run locally

```sh
git clone https://github.com/pumpajjj/pumpajjj.git
cd pumpajjj
python3 -m http.server 8000
```

Then open <http://localhost:8000>. (You can also open `index.html` directly, but a local server avoids browser restrictions on loading audio.)

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app: markup, SVG pump, styles and script |
| `bg.png` | Tiled background pattern |
| `brnaba.png`, `vucic.png`, `vucevic.png` | Balloon images |
| `pumpaj.png`, `pumpaj.mp3` | Bonus image and sound shown every 5 balloons |
| `bicyclepump.mp3`, `pop.mp3` | Pump and pop sound effects |
| `support-students.svg` | Donation button icon |
| `preview.png` | Social media preview image |

## Deployment

Hosted on GitHub Pages straight from the repository root. Push to the default branch and the site updates.

## Contributing

Issues and pull requests are welcome. Keep it simple: one HTML file, no dependencies.

**Pumpaj!** 🚲🎈

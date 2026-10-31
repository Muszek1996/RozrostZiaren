# RozrostZiaren

Browser grain growth simulation ("rozrost ziaren" is Polish for grain growth) built as a 2D cellular automaton on a canvas. Grains (nuclei) start on the grid and grow into empty cells from their von Neumann neighbours.

- Nucleation modes: uniform, with radius, random, or manual (click on the canvas)
- Grid size, nuclei count, speed and periodic boundary conditions are set in the UI
- `src/`: ES6 source (`Board.js`, `Cell.js`, `index.js`, `index.html`); `dev/`: Babel output

The follow-up version, with more neighbourhoods, Monte Carlo growth and recrystallization, is [RozrostZiarenCD](https://github.com/Muszek1996/RozrostZiarenCD).

## Build & run
```bash
npm install
npm install -g watchify     # used by the bundle script
npm run build               # babel src -> dev, bundle -> dist/bundle.js
```
Open `dist/index.html` in a browser.

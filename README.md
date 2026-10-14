# EV 3D Engine

Interactive 3D EV traction motor and drive unit, built with Three.js and running entirely in the browser.

**Live demo:** https://rebelionseo.github.io/EV-3D-Engine/

## Features

- **3D EV Autoshop dyno bay**: the drive unit sits on a dyno in a modeled workshop scene you can orbit, pan and zoom.
- **Exploded views**: pull the assembly apart to see the stator, rotor, housing, gearbox and inverter on their own.
- **90° CAD section cutaways**: quarter-section views that show the internal structure, like a CAD cutaway.
- **Synthesized acoustics**: SiC inverter whine and motor sound are generated live with the Web Audio API, with no audio files.
- **Accelerator and brake pedals**: interactive controls that drive the motor, with 0–60 MPH telemetry.

## Tech

- [Three.js](https://threejs.org/) r128 with OrbitControls
- Web Audio API
- Tailwind CSS (CDN), Font Awesome, Google Fonts

There's no build step. Everything lives in `index.html`.

## Run locally

Open `index.html` in a modern browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

Audio starts after your first click or keypress, because browsers block autoplay.

## Deployment

GitHub Pages serves the site from the root (`/`) of the `main` branch.

# Golden Gate Bridge — Cinematic Simulation

A self-contained, high-fidelity 3D simulation of the Golden Gate Bridge and San Francisco Bay, built with **Three.js**. No build step — open one HTML file in Chrome.

![Golden Gate Bridge](https://img.shields.io/badge/Three.js-r160-blue) ![License](https://img.shields.io/badge/license-MIT-green)

## Features

- **Golden Gate Bridge** — Art-deco towers, Warren truss deck, main cables, suspenders, anchorages, approach viaducts, tunnel portals
- **San Francisco skyline** — Instanced buildings, landmarks (Transamerica Pyramid, Salesforce Tower, Coit Tower), night window lights
- **Marin Headlands** — Golden hills, groves, beaches, Angel Island, Alcatraz
- **Dynamic atmosphere** — Physical sky (Preetham), drifting clouds, horizon haze, volumetric fog sprites, stars & moon
- **Water** — Gerstner waves, planar reflections, shore tide, foam
- **Traffic & ships** — Instanced cars (4 vehicle types), cargo ships with wakes, flocking birds
- **Time of day** — Full 24h cycle with dawn, golden hour, dusk, and night lighting
- **Post-processing** — ACES tone mapping, bloom, vignette, film grain
- **Cinematic tour** — 12-shot automated flythrough (~92s) with transitions and title card

## Quick Start

1. Clone this repository
2. Open `golden_gate_bridge.html` in **Chrome** (or any modern browser with WebGL)
3. Use the control panel (top-left) or drag to orbit the scene

No `npm install`, no bundler, no server required.

## Controls

| Input | Action |
|-------|--------|
| **Drag** | Orbit camera |
| **Scroll** | Zoom |
| **Right-drag** | Pan |
| **Time slider** | 0–24h time of day |
| **Fog / Traffic / Zoom** | Scene parameters |
| **▶ CINEMATIC TOUR** | Play the automated trailer |
| **ESC** | Exit cinematic mode |

## Tech Stack

- [Three.js](https://threejs.org/) r160 (ES modules via CDN import map)
- Custom GLSL shaders (water, sky haze, post FX)
- Procedural canvas textures (no external image assets)
- `InstancedMesh` for trees, buildings, cars, street lights

## Project Structure

```
goldenbridge/
├── golden_gate_bridge.html   # Entire app — HTML + CSS + JS in one file
├── README.md
└── LICENSE
```

## License

MIT — see [LICENSE](LICENSE).

## Acknowledgments

Inspired by the real Golden Gate Bridge and San Francisco Bay. Built as a visual simulation / art piece, not a geographic survey.

# AI Generated Projects

An independent collection of AI-assisted code experiments, visual simulations, and interactive demos.

**Live website (GitHub Pages):** https://chinhbui.github.io/ai-generated-projects/

## Projects

| Project | Description | Demo | Source |
| --- | --- | --- | --- |
| BMW Inline-Six Engine | Interactive 2D cutaway of an inline-six engine, with a four-stroke cycle, synchronized piston/crank motion, and an RPM control. | [Open demo](https://chinhbui.github.io/ai-generated-projects/projects/bmw-inline-six/) | [HTML](projects/bmw-inline-six/index.html) |
| F-35A Acceleration & Dive | 3D educational flight scene: acceleration, push-over, steep dive, pull-up, three cameras, throttle and flight instruments. | [Open demo](https://chinhbui.github.io/ai-generated-projects/projects/f35-flight-simulator/) | [HTML](projects/f35-flight-simulator/index.html) |

## Repository structure

```text
.
├── index.html                         # Project catalog / GitHub Pages homepage
├── projects/
│   ├── bmw-inline-six/
│   │   └── index.html                 # Standalone engine animation
│   └── f35-flight-simulator/
│       └── index.html                 # Interactive 3D flight scene
└── README.md
```

Each new demo should live in `projects/<project-slug>/` with an independent entry point (preferably `index.html` for browser demos). Link it from the root `index.html` and catalog above.

## GitHub Pages

This repository serves static HTML with no build step or workflow. The BMW demo is standalone; the F-35A demo loads a pinned Three.js ES module from jsDelivr at runtime (internet connection required).

Configure **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main → Folder: /(root) → Save**. The site then publishes on pushes to `main`.

## Notes

- These projects were created with AI assistance for learning and experimentation; they are not production-validated.
- The BMW simulation is educational, not an official BMW product or an engineering-grade CAD model.
- The F-35A model uses the published 15.7 m length and 10.7 m wingspan, but its motion model is illustrative and is **not** a certified flight simulator or validated F-35 aerodynamics. A modern browser supporting WebGL and ES modules is required.
- F-35A controls: pause/resume, replay, dive now, chase/side/top views, thrust slider (50–100%). Space = pause/resume, R = replay, 1/2/3 = views. Source for dimensions: https://www.lockheedmartin.com/content/dam/lockheed-martin/aero/documents/F-35/f35A.pdf
- No license has been granted by this README. Add a `LICENSE` file when you decide the project's license.

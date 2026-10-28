# AI Generated Projects

An independent collection of AI-assisted code experiments, visual simulations, and interactive demos.

**Live website (GitHub Pages):** https://chinhbui.github.io/ai-generated-projects/

## Projects

| Project | Description | Demo | Source |
| --- | --- | --- | --- |
| BMW Inline-Six Engine | Interactive 2D cutaway of an inline-six engine, with a four-stroke cycle, synchronized piston/crank motion, and an RPM control. | [Open demo](https://chinhbui.github.io/ai-generated-projects/projects/bmw-inline-six/) | [HTML](projects/bmw-inline-six/index.html) |

## Repository structure

```text
.
├── index.html                         # Project catalog / GitHub Pages homepage
├── projects/
│   └── bmw-inline-six/
│       └── index.html                 # Standalone animation
└── README.md
```

Each new demo should live in `projects/<project-slug>/` with an independent entry point (preferably `index.html` for browser demos). Link it from the root `index.html` and catalog above.

## GitHub Pages

This repository serves plain static HTML. No build step, dependencies, or workflow are required.

Configure **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main → Folder: /(root) → Save**. The site then publishes on pushes to `main`.

## Notes

- These projects were created with AI assistance for learning and experimentation; they are not production-validated.
- The BMW simulation is educational, not an official BMW product or an engineering-grade CAD model.
- No license has been granted by this README. Add a `LICENSE` file when you decide the project's license.

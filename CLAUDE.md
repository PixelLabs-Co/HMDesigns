# HM Design site

- This repo is `hm-designs/hm-designs.github.io`, owned by the **`hm-designs`** GitHub account. It is published with GitHub Pages at https://hm-designs.github.io (branch `main`, root).
- It is a **separate project and separate GitHub account** from the Pixel Labs site (`PixelLabs-Co/pixelabs-site`). Never push HM Design work to the Pixel Labs repo, or Pixel Labs work to this one.
- Plain static HTML/CSS/JS: `index.html`, `fonts/`, `portfolio/` (project images), `store/` (shop product images), `hero/` (hero collage artwork), `logo-v3.png`, `harrison.jpg`. No build step.
- Design: black and warm off-white (`--paper` #E7E4DF, with slightly darker `--paper-2` for the Shop sheet and form panel), bold and minimalist. Project images are shown in colour. The one accent is the lime "available for work" dot in the About section.
- Adding or editing projects: follow the "To add new work" comment above `#portfolioGrid` in `index.html`.
- The Shop section is generated: `.github/workflows/update-store.yml` runs `scripts/update_store.py` every 6 hours, reads the Gumroad profile, and rewrites the block between the `shop:start` / `shop:end` markers in `index.html` plus `store/` images. Don't hand-edit that block; pin wording for a product in `store/overrides.json` (keyed by Gumroad permalink).

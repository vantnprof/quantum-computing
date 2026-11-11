# Quantum Computing Course

Course website built with [Jupyter Book](https://jupyterbook.org) and deployed to GitHub Pages.

## Run the website locally

```bash
python3 -m venv .venv
source .venv/bin/activate          # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter book start                 # live preview at http://localhost:3000
```

Pages reload automatically when you edit files. Stop the server with `Ctrl+C`.
Jupyter Book needs [Node.js](https://nodejs.org) (v20+); if it is missing, it will offer to install it.

To build the static site (the same output GitHub Pages serves): `jupyter book build --html`
(the result is in `_build/html/`).

`requirements.txt` also installs the quantum stack used in the lectures (NumPy, Matplotlib, Qiskit, Qiskit Aer).

## Structure

- `myst.yml`: book configuration, table of contents and math macros (`\ket`, `\bra`, `\braket`)
- `index.md`: home page (hero, roadmap, how to use the course)
- `lectures/NN-topic/index.md`: one folder per lecture. Put slides, notebooks and materials in the same folder
- `.github/workflows/deploy.yml`: builds and deploys the site on every push to `main`

## Themes

Two themes live in `assets/themes/`, each with its own `custom.css`, logos and favicon:

| Theme | Look |
| --- | --- |
| `detective` (active) | Navy and crimson case files: searchlight hero with a magnifying glass, a cork evidence board with pinned cards and red string, "Case NN" folders, SOLVED / UNSOLVED stamps |
| `cosmic` | Deep-space violet and cyan: starfield hero, glowing orbit, neon gradients |

To switch, replace the theme folder name in the four paths under `site.options` in `myst.yml`
(`logo`, `logo_dark`, `favicon`, `style`).

## Customising the look

- `assets/themes/<theme>/custom.css`: colours, fonts, hero, roadmap, lecture banners and footer.
  Phase colours are the `--phase-1` … `--phase-6` variables at the top
- `assets/themes/<theme>/logo.svg`, `logo-dark.svg`, `favicon.png`: branding
- `parts/footer.md`, `parts/sidebar-footer.md`: site footer and sidebar footer
- `myst.yml` → `site.nav` / `site.actions`: top navigation links and buttons

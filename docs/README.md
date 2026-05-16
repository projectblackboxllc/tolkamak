# Tolkamak — Website (GitHub Pages bundle)

Static site companion to the Zenodo deposit *A Toroidal Geometric Rectifier: Empirical Disproof of Linear-Response in Plasma Confinement* (v1.2, DOI [10.5281/zenodo.20245905](https://doi.org/10.5281/zenodo.20245905)).

**Live site:** https://projectblackboxllc.github.io/tolkamak/

## Files

- `index.html` — landing page (project overview, headline result, embedded sim, Dirty-Twin benchmark walkthrough, industries, citation).
- `sim.html` — interactive standalone visualization. Drag the drive slider to see the saturating-homeostat snap into geometric lock above the threshold. Embedded in `index.html` via `<iframe>`. Also linkable as its own page.
- `style.css` — shared site styling (dark theme, GitHub-flavored palette).
- `assets/` — figures referenced in the page:
  - `fig_002_homeostat_attractor.png` — headline figure (309% / 7% drive-invariance result)
  - `fig_003_dirty_twin_blindness.png` — sensor sparsity + latency benchmark
  - `fig_004_dirty_twin_slew.png` — actuator slew-rate benchmark
  - `fig_006_dirty_twin_ripple_stringent.png` — stringent ripple test (parallel-dominant)

## Deployment

This `docs/` directory is the GitHub Pages source for the `tolkamak` repository. Pages is configured to serve from `main` branch `/docs` — see repo Settings → Pages. To deploy a custom domain later, add a `CNAME` file to this folder.

## Local preview

```bash
cd docs/
python3 -m http.server 8000
# Open http://localhost:8000 in a browser.
```

## License and attribution

License terms are attached to the Zenodo deposit metadata rather than declared on the site itself. The interactive simulation is a qualitative visualization of empirically-measured behavior; the underlying control-law mathematics is held proprietary.

Andrew Woodward — Project Black Box LLC · CAGE 11FU4
ORCID: [0009-0006-9717-7161](https://orcid.org/0009-0006-9717-7161)
Source: [github.com/projectblackboxllc](https://github.com/projectblackboxllc)

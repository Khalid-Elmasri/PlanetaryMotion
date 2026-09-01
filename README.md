# PlanetaryMotion

Interactive Jupyter notebook exploration of orbital mechanics and planetary motion — numerical simulations, visualisations, and experiments in gravitational dynamics collected in a single, runnable notebook.

## Contents
- `planetary_motion.ipynb` — primary notebook with explanations, simulations, plots, and (where applicable) animations demonstrating two-body and multi-body orbital dynamics, numerical integrators, parameter studies, and visual diagnostics.
- `README.md` — this file.

## Goals
- Demonstrate how simple physical laws (Newtonian gravity / Keplerian motion) produce planetary orbits.
- Show how numerical integrators behave (symplectic vs. non-symplectic), trade-offs in accuracy vs. cost, and how to visualise conservation properties (energy, angular momentum).
- Provide interactive examples you can run, modify, and extend for classroom use or personal exploration.

## Requirements
- Python 3.8+ recommended
- Jupyter (Notebook or JupyterLab)
- Typical scientific Python stack:
  - numpy
  - scipy
  - matplotlib
  - pandas (optional, for tables)
  - astropy (optional, for physical units and constants)
  - ipywidgets (optional, for interactive controls)
  - tqdm (optional, for progress bars)

Suggested quick-install (venv + pip):
```bash
python -m venv .venv
source .venv/bin/activate     # on Windows: .venv\Scripts\activate
pip install --upgrade pip
pip install jupyterlab numpy scipy matplotlib pandas astropy ipywidgets tqdm

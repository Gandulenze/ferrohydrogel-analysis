# Analysis code — Master thesis

Python code used for the data analysis in the master thesis

> *One-Step Synthesis of Ferrohydrogels by High-Energy Electron-Beam Irradiation:
> Experiments and Characterization*
> Leibniz Institute of Surface Engineering (IOM) / Leipzig University, 2026

The notebooks reproduce the fits and figures shown in the thesis. Each one is
self-contained and configured through a small block of settings at the top of
the relevant cell (file names, fit windows, sample mass, plot options).

## Contents

| Notebook | Purpose |
| --- | --- |
| `Pulsradiolysis_Plot.ipynb` | Transient absorption data: extraction of kinetic traces at a chosen probe wavelength, mono-exponential fits of the observed rate constants, and the weighted linear fit yielding the second-order rate constant. Also produces the transient absorption spectra. |
| `XRD_Plot.ipynb` | Powder diffractograms with magnetite / hematite / halite reference reflections, pseudo-Voigt fits of individual reflections, lattice parameters from the fitted positions, and the Scherrer crystallite size from the (311) reflection. |
| `VSM_Plots.ipynb` | Magnetometry data: empty-holder background subtraction, conversion from CGS to SI and to mass-specific magnetization, coercive field and remanence, Langevin fit with a linear high-field term, and ZFC / FC curves. |

## Data

The raw measurement data are **not** included in this repository. The notebooks
expect the corresponding files in the paths set at the top of each notebook
(e.g. `DATA_DIR` for the pulse-radiolysis CSV files, `TS1/Hysterese` and
`TS2/ZFC-FC` for the PPMS `.dat` files). The code is published for documentation and transparency rather than as a
ready-to-use analysis package.

## Requirements

Python 3.12 with `numpy`, `scipy`, `pandas` and `matplotlib`:

```bash
pip install numpy scipy pandas matplotlib
```

## Note on AI assistance

This code was written with the assistance of AI-based tools (Anthropic Claude,
OpenAI ChatGPT). All models, fit procedures and analysis decisions were
specified, reviewed and verified by the author.

## License

MIT — see [LICENSE](LICENSE).

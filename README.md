# Magnetic Field in the Universe

A **Python‑based central manager** for working with observational surveys of cosmic magnetic fields. Instead of hosting large data files, this repo gives you the **scripts, parsers, and notebooks** you need to download, standardize, and compare datasets from the literature (dust polarimetry, Zeeman splitting, Faraday rotation, and more).

---

## Goals

* Provide **reproducible Python pipelines** that turn publication data products into clean, science‑ready tables on your own machine.
* Make it simple to **build your data collection** and keep it in sync with new survey releases.
* Enable **cross‑comparison** between magnetic‑field-related quantities from different publications or surveys.
* Serve as a lightweight, community‑maintained magnetic field research knowledge base.

---
## Repository layout ***(proposed)***

```
magnetic-fields-universe/
├── data/                      # User‑local copies of survey products (ignored by git)
│   ├── polarization/          # CSO, JCMT, ALMA, Planck, …
│   ├── zeeman/                # Crutcher catalog, OH/NH3, …
│   └── faraday/               # RM grids, LOFAR, ASKAP, …
│
├── scripts/                   # Python helpers
│   ├── fetch_*.py             # Downloaders
│   ├── parse_*.py             # Convert raw ASCII → tidy CSV, TXT, …
│   └── make_*.py              # Combine & clean datasets
│
├── notebooks/                 # Jupyter demo notebooks
│   └── 00_quickstart.ipynb    # 15‑min tour of the toolbox
│
├── docs/                      # Longer‑form docs & rendered HTML
│   └── polarization_density_db/
│
├── tests/                     # Unit tests for parsers
├── examples/                  # Mini‑projects / tutorials
├── requirements.txt           # Core Python deps (numpy, astropy, pandas, …)
├── environment.yml            # Conda env (optional)
├── CONTRIBUTING.md            # How to add code or docs
├── LICENSE                    # MIT
└── README.md                  # ← you are here
```

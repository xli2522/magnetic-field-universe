# Magnetic Field in the Universe

A **Python‑based data manager** for working with tabulated data from publications of observational surveys of cosmic magnetic fields. Instead of hosting large data files, this repo gives you the **scripts, parsers, and notebooks** you need to download, standardize, and compare datasets from the literature (dust polarimetry, Zeeman splitting, Faraday rotation, and more).

---

## Goals

* Provide **reproducible Python pipelines** that turn publication data products into clean, science‑ready tables on your own machine.
* Make it simple to **build your data collection** and keep it in sync with new survey releases.
* Enable **cross‑comparison** between magnetic‑field-related quantities from different publications or surveys.
* Serve as a lightweight, community‑maintained magnetic-field-in-the-universe research knowledge base.

---
## Repository layout ***(proposed)***

```
magUniverse-master
│── maguniverse/
│   ├── data/                  # Get raw data and convert to tidy CSV, TXT, … 
│   │   ├── polarization/      # CSO, JCMT, ALMA, Planck, …
│   │   ├── zeeman/            # Crutcher catalog, OH/NH3, …
│   │   └── faraday/           # RM grids, LOFAR, ASKAP, …
│   │
│   ├── utils/                 # Python helpers
│   │   └── fetch_*.py         # Downloaders
│   │
│   └── datafiles/             # User copy of data
│
├── notebooks/                 # Jupyter demo notebooks
│   └── 00_quickstart.ipynb    # 15‑min tour of the toolbox
│
├── docs/                      # Longer‑form docs & rendered HTML
│   └── maguniverse/
│
├── tests/                     # Unit tests for parsers
├── examples/                  # Mini‑projects / tutorials
├── requirements.txt           # Core Python deps
├── CONTRIBUTING.md            # How to add code or docs
├── LICENSE                    # MIT
└── README.md                  # ← you are here
```

# Longitudinal Asymmetry and Local-Time Dependence of Geomagnetic Cutoff Rigidity Depression During the May 2024 Superstorm

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22818267.svg)](https://doi.org/10.5281/zenodo.22818267)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MustakimSaron/May2024-Cutoff-Rigidity-Asymmetry/blob/main/cosmoshield_inversion_pipeline.ipynb)

This repository provides the complete computational inversion scheme, observational datasets, and statistical scripts supporting the manuscript:

> **Md Mustakim Bin Alam**, *"Longitudinal Asymmetry and Local-Time Dependence of Geomagnetic Cutoff Rigidity Depression During the May 2024 Superstorm"*, Department of Physics, Novosibirsk State University (*Submitted to Geomagnetism and Aeronomy*).

---

## Scientific Overview

During extreme space weather events, ring current intensification inflates Earth's magnetic dipole, lowering the geomagnetic cutoff rigidity ($\Delta R_c < 0$) and allowing lower-energy primary cosmic rays to penetrate mid-latitude atmospheres. 

While classical models assume globally uniform shielding depression parameterized by $SYM\text{-}H$, this pipeline decouples heliospheric Forbush decreases from magnetospheric cutoff shifts to demonstrate an acute **longitudinal asymmetry ($\Xi(t) = \Delta R_{c,\mathrm{MOSC}} - \Delta R_{c,\mathrm{NEWK}} = -1.04\text{ GV}$)** during the May 10–12, 2024 G5 superstorm. 

Phase-space diagnostics show that this asymmetry exhibits single-valued dynamic tracking with the partial ring current index ($ASYM\text{-}H$, $R^2 = 0.810$), while forming an open hysteresis loop against $SYM\text{-}H$.

---

## Repository Structure

```text
May2024-Cutoff-Rigidity-Asymmetry/
│
├── cosmoshield_inversion_pipeline.ipynb  # Executable reproduction notebook
├── run_inversion.py                      # Standalone Python inversion pipeline
├── requirements.txt                      # Core dependencies
├── README.md                             # Repository documentation
│
├── data/
│   ├── may2024_superstorm_inversion_timeseries.csv # Master 1-hour time series
│   ├── table1_station_summary.csv                  # Station metadata and peak extrema
│   └── table2_regression_metrics.csv               # Linear fit parameters
│
└── figures/
    ├── cutoff_rigidity_asymmetry_fixed.png         # Figure 1: Inversion overview
    ├── fig2_combined_hysteresis_correlation.png    # Figure 2: Kyoto index dynamics
    ├── fig3_spectral_sensitivity.png               # Figure 3: Rigidity index invariance
    └── fig4_aeronomic_ionization_impact.png        # Figure 4: Mesospheric ionization collapse

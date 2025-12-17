# Quantifying Detection Biases in the TESS Exoplanet Survey

## Overview
Transit surveys such as **TESS** do not provide an unbiased view of the exoplanet population.
Detection and confirmation probabilities depend on planet radius, orbital period, and
limitations in follow-up observations. This project quantifies those selection effects
using publicly available catalogs.

This analysis is fully reproducible and uses programmatic access to the NASA Exoplanet
Archive.

---

## Data Sources
- **NASA Exoplanet Archive** confirmed planets
- **TESS Objects of Interest (TOI)** catalog
- TESS Input Catalog (via Exoplanet Archive)

Raw catalog data are *not* stored in this repository. They are obtained dynamically
during notebook execution.

---

## Key Figures

### 1) TESS Candidates vs Confirmed Planets

Shows detected candidates (blue) vs confirmed planets (orange) in period–radius space.

![Candidates vs Confirmed](docs/figures/candidates_vs_confirmed.png)

---

### 2) Confirmation Efficiency vs Planet Radius

Confirmation efficiency as a function of planet radius reveals systematic
bias against small and very large planets.

![Efficiency vs Radius](docs/figures/efficiency_vs_radius.png)

---

### 3) Confirmation Efficiency vs Orbital Period

Shows how efficiency varies with orbital period, reflecting false-positive
rates at short periods and fewer transits at long periods.

![Efficiency vs Period](docs/figures/efficiency_vs_period.png)

---

### 4) Observed vs Bias-Corrected Radius Distribution

Correcting for confirmation bias reveals an enhanced population of small planets
compared to the confirmed sample.

![Observed vs Corrected](docs/figures/observed_vs_corrected_radius.png)

---

### 5) 2D Confirmation Efficiency Map

A heatmap of confirmation efficiency across period–radius space. Regions with sparse
data are masked to avoid overinterpretation.

![Completeness Map](docs/figures/completeness_map.png)

---

## Additional Supporting Figure

### Bias-Corrected Radius Distribution with Uncertainty

Shows propagated binomial uncertainties in the corrected planet counts.

![Bias Corrected with Uncertainty](docs/figures/bias_corrected_radius_uncertainty.png)

---

## Methodology Summary

1. Ingest confirmed and candidate exoplanet catalogs.
2. Compare confirmed planets and TOI candidates in period–radius space.
3. Compute confirmation efficiency as a function of planet radius and orbital period.
4. Propagate binomial uncertainties into efficiency estimates.
5. Build a 2D completeness map in period–radius space.
6. Correct the observed distribution for confirmation bias.

---




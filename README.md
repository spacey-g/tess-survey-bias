# tess-survey-bias
Quantifying detection biases in the TESS exoplanet survey
# Quantifying Detection Biases in the TESS Exoplanet Survey

## Motivation
Transit surveys such as TESS do not provide an unbiased view of the exoplanet population.
Detection probability depends strongly on stellar brightness, noise properties, orbital period,
and planet size. Understanding these selection effects is essential for inferring true
planet occurrence rates.

This project aims to quantify detection biases in the TESS survey using public catalogs
and reproducible statistical methods.

## Data Sources
- NASA Exoplanet Archive
- TESS Objects of Interest (TOI) catalog
- TESS Input Catalog (TIC)

## Objectives
- Characterize detection efficiency as a function of planet and stellar properties
- Visualize survey completeness in period–radius space
- Explore bias-corrected exoplanet population trends

## Repository Structure
- `data/` : raw and processed catalogs
- `notebooks/` : analysis notebooks
- `src/` : reusable analysis utilities
- `results/` : figures and tables

## Status
🚧 Initial development — catalog ingestion and exploratory analysis

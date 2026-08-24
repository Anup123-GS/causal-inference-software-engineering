# Techniques for Inferring Causal Effects in Software Engineering Research

## Author
Anup Gururaj Shastry  
MSc Data Science and Analytics  
University College Cork  
2026

## Project Overview
This repository contains the code and datasets used in the dissertation
"Techniques for Inferring Causal Effects in Software Engineering Research."

GitHub Actions adoption is used as an empirical case study to compare causal
inference techniques using observational software-repository data.

## Methods
The analysis includes:

- Regression Adjustment (OLS)
- Custom distance-based matching
- Propensity Score Matching using PsmPy
- Difference-in-Differences (DiD)
- Event-study analysis
- Placebo and sensitivity analyses
- Doubly Robust Difference-in-Differences (DR-DiD)

## Repository Structure

- `notebook/` – Final Jupyter notebook containing the analysis
- `data/` – Datasets used and generated during the analysis
- `requirements.txt` – Required Python packages

## GitHub API Authentication

GitHub API requests require a personal access token.

The token is NOT stored in the notebook or dataset.

In Google Colab, create a secret named:

`GITHUB_TOKEN`

Alternatively, when running locally, set `GITHUB_TOKEN` as an environment
variable.

## Reproducibility

The final analysis uses repositories satisfying the required pre-treatment
and post-treatment observation windows at the analysis cutoff of
24 August 2026.

Because GitHub repository metadata can change over time, rerunning the
upstream GitHub API collection at a later date may produce slightly different
candidate repositories or metadata.

The supplied datasets preserve the data used for the submitted analysis.

## Software

The analysis was conducted in Python using packages including pandas,
NumPy, scikit-learn, statsmodels, PsmPy and linearmodels.

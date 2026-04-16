# Monte Carlo Life Insurance Simulation

A Monte Carlo simulation of human lifetimes built on CDC actuarial life table data. Simulates 10,000 random lifetimes to model survival probabilities, expected remaining life, and insurance payouts — then validates results against theoretical life table values.

---

## Overview

Life insurance pricing relies on actuarial models that estimate how long people are likely to live. This project uses Monte Carlo methods to simulate individual lifetimes year-by-year based on real mortality probabilities, showing how population-level patterns emerge from individual randomness.

---

## What It Does

- Loads CDC life table data (age-specific death probabilities `qx`)
- Simulates 10,000 random lifetimes using year-by-year Bernoulli trials
- Computes survival curves, expected remaining lifetime, and estimated insurance payouts
- Compares empirical Monte Carlo results against closed-form theoretical values
- Visualizes results with histograms and survival curve overlays

---

## Key Results

- Simulated lifetime distribution peaked in the **late 70s to early 80s**, consistent with U.S. mortality data
- Empirical survival curve converged closely with the theoretical curve across all age groups
- Expected remaining lifetime followed the expected pattern — high at birth, declining faster in later years

---

## Files

| File | Description |
|------|-------------|
| `project6_mth337.ipynb` | Main Jupyter notebook with full simulation and analysis |
| `life_table.csv` | CDC life table data (age, `qx`) |

---

## Stack

Python · NumPy · Matplotlib

---

## Data Source

[CDC National Life Tables](https://www.cdc.gov/nchs/products/life_tables.htm)

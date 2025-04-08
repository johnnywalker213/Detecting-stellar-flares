# Detecting Stellar Flares Using Conditional Volatility

[![Paper Status](https://img.shields.io/badge/status-accepted-brightgreen)](https://doi.org/XXXX) 
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

A robust method to detect stellar flares in TESS light curves by combining harmonic detrending and stochastic volatility modeling (GARCH).

## Description

This repository hosts the code for the paper *"Detecting stellar flares in the presence of a deterministic trend and stochastic volatility"*. The method:
1. **Removes deterministic trends** in light curves using a time-varying harmonic model.
2. **Models stochastic volatility** (residual fluctuations) using techniques from econometrics (GARCH).
3. **Detects flares** as statistically significant outliers in the volatility-adjusted residuals.

Applied to TESS observations of two stars, the method detected **146–462 flares** with energies as low as **7×10²⁸ erg/s**, revealing distinct power-law energy distributions.


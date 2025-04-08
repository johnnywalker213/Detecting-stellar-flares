# Detecting Stellar Flares Using Conditional Volatility

[![Paper Status](https://img.shields.io/badge/status-accepted-brightgreen)](https://doi.org/XXXX) 
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

A robust method to detect stellar flares in TESS light curves by combining harmonic detrending and stochastic volatility modeling (GARCH).

## Description

This repository hosts the code for the paper *"Detecting stellar flares in the presence of a deterministic trend and stochastic volatility"* by  
Qiyuan Wang, Giovanni Motta, Genaro Sucarrat, and Vinay Kashyap  
(Departments and Institutions as listed in the paper). The method:
1. **Removes deterministic trends** in light curves using a time-varying harmonic model. We remove the non-stochastic baseline using a harmonic model with time-varying amplitudes. This approach adapts to variations in the underlying stellar emission, ensuring that the residuals represent the true stochastic behavior.
2. **Models stochastic volatility** (residual fluctuations) using techniques from econometrics (GARCH). The stochastic component of the light curves is modeled similarly to financial time series. We adopt GARCH processes to effectively capture the volatility clustering and to distinguish the impulsive flares from background noise.
3. **Detects flares** as statistically significant outliers in the volatility-adjusted residuals. By comparing the observed signal with the predicted baseline volatility, flares are detected as statistically significant deviations. The method has been tested on two distinct cases:
   TIC-1 (G5V eruptive variable): Up to 146 flares detected.
   TIC-2 (M4 high-proper motion star): Up to 462 flares detected.
Flares are further characterized by their frequency and energy distributions, with power-law exponents of approximately 1.85 and 2.1, respectively.

## Contact
For any questions, issues, or suggestions, please contact:
Qiyuan (Johnny) Wang： wqy213@tamu.edu



# VECM-VAR Forecasting Financial Instruments

A time series forecasting project analyzing financial instrument prices using **Vector Error Correction Model (VECM)** and **Vector Autoregression (VAR)**. It includes full pipeline from data import, stationarity testing, cointegration testing, model building, diagnostics, forecasting, and performance evaluation.

---

## 🔍 Overview

This repository contains a detailed Jupyter-based analysis and implementation of a time series forecasting workflow for financial instruments. The project performs:

- Exploratory data analysis and differencing
- Stationarity testing with the Augmented Dickey-Fuller (ADF) test
- Pairwise OLS regression for residual analysis
- Johansen cointegration test to identify long-run relationships
- Estimation of VECM with short- and long-run dynamics
- Model diagnostics (autocorrelation, normality)
- Reparameterization of VECM as VAR
- Forecasting and error evaluation (MAE, MAPE, etc.)
- Impulse Response Functions (IRF) and Forecast Error Variance Decomposition (FEVD)

---

## 📁 Files

- `TSA_2025_project_data_1.csv`: Input time series dataset with 10 financial instrument series
- `main_notebook.ipynb`: Full pipeline with explanations, tests, and visualization
- `README.md`: Project documentation

---

## 📊 Forecasting Techniques

| Technique        | Description |
|------------------|-------------|
| **ADF Test**      | For checking unit roots and stationarity of series |
| **Johansen Test** | For detecting cointegrated relationships among variables |
| **VECM**          | To capture both long-run equilibrium and short-run dynamics |
| **VAR**           | For vector autoregressive modeling and forecasting |
| **IRF/FEVD**      | For interpreting shock dynamics and source of variances |

---

## 🧪 Forecasting Results (Highlights)

- Forecasting horizon: 25 periods
- X MAPE: ~3.92%, Y MAPE: ~2.43%
- Residuals: No autocorrelation, approximately normal
- X drives Y in long-run and short-run dynamics
- System is stable and well specified

---

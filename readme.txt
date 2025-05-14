# Time Series Modeling with ARIMA & SARIMA

## Project Goals

* Forecast NVIDIA (NVDA) stock closing prices using ARIMA and SARIMA models.
* Compare the performance of ARIMA vs. SARIMA and select the best model.
* Demonstrate a complete time series analysis workflow: data retrieval, EDA, decomposition, modeling, and evaluation.

## Overview

This repository contains a Jupyter Notebook and supporting scripts to:

1. **Load and visualize** historical stock data for NVIDIA via Yahoo Finance.
2. **Decompose** the time series into trend, seasonal, and residual components (STL).
3. **Test stationarity** (ADF test) and apply differencing if needed.
4. **Identify model orders** using ACF and PACF plots.
5. **Fit ARIMA** and **SARIMA** models to log-transformed data.
6. **Forecast** future stock prices and evaluate model accuracy.
7. **Diagnose residuals** and **compare error metrics** (RMSE, MAE, MAPE) and information criteria (AIC/BIC).
8. **Select the best model** based on parsimony and performance.

## How to Run

1. **Clone the repo**:

   ```bash
   git clone https://github.com/your_username/time-series-arima-sarima.git
   cd time-series-arima-sarima
   ```
2. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```
3. **Execute the notebook**:

   * Open `notebooks/ARIMA_SARIMA_Modeling.ipynb` in Jupyter Lab/Notebook.
   * Run all cells sequentially.
4. **Or run scripts**:

   ```bash
   python scripts/preprocessing.py
   python scripts/modeling.py
   ```
5. **View results** in `results/figures/` and `reports/`.

---

For detailed instructions and interpretations, refer to the individual markdown sections in the notebook.

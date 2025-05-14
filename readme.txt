#Time Series Modeling with ARIMA & SARIMA  📈 

## 🎯 Project Goals
- 📊 Forecast **NVIDIA (NVDA)** stock closing prices using ARIMA and SARIMA models.
- ⚖️ Compare model performance and select the best fit.
- 🧠 Demonstrate an end-to-end time series analysis workflow:
  - Data retrieval
  - Exploratory Data Analysis (EDA)
  - Decomposition
  - Modeling
  - Evaluation

---

## 📚 Overview

This repository includes a Jupyter Notebook and supporting scripts to:

1. 📥 Load and visualize historical NVIDIA stock data using **Yahoo Finance**.
2. 🧩 Decompose the time series into **trend**, **seasonal**, and **residual** components using STL.
3. 🧪 Conduct **stationarity testing** (ADF test) and apply differencing if required.
4. 🧠 Identify model parameters using **ACF/PACF** plots.
5. 🤖 Fit **ARIMA** and **SARIMA** models on log-transformed data.
6. 🔮 Forecast future stock prices and evaluate accuracy.
7. 🩺 Diagnose residuals and compare:
   - Error metrics: **RMSE, MAE, MAPE**
   - Information criteria: **AIC, BIC**
8. 🏆 Select the best model based on parsimony and performance.

---

## 🚀 How to Run

### 🔧 Step 1: Clone the repo
```bash
git clone https://github.com/your_username/time-series-arima-sarima.git
cd time-series-arima-sarima


📁 Step 5: View results
📊 Figures will be saved in: results/figures/

📝 Reports, logs, and notes: reports/

📖 Notes
The notebook contains markdown cells that explain:

What each modeling step is doing

How the diagnostics work

How metrics were chosen

This can serve as a good learning reference for others, too.

🙋‍♀️ Questions or Suggestions?
Open an issue or create a discussion.

⭐ Support
If you find this project helpful:

Give it a ⭐ star on GitHub

Share with others interested in time series forecasting!

🧠 Credits
pmdarima for auto_arima

statsmodels for SARIMAX implementation

Yahoo Finance via yfinance for stock data

All visualizations created using matplotlib and seaborn

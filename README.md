## Time Series Modeling with ARIMA & SARIMA (NVIDIA)  

## 🏆 Motivation
- I’ve spent considerable time studying global technological history, economics, and geopolitics. The ongoing silicon (semiconductor) revolution—driven by companies like NVIDIA, TSMC, and ASML—is something my peers and I anticipated nearly a decade ago. This project aims to quantitatively explore that shift by building an end-to-end ARIMA/SARIMA model to forecast NVIDIA's stock prices.

## 🧩 WHY only ARIMA/SARIMA for this TIME series, why not LSTM, GRU, Prophet?
- For this project, ARIMA and SARIMA were chosen due to their effectiveness on smaller, univariate datasets like stock closing prices. They offer strong interpretability, are easy to implement, and require fewer computational resources compared to deep learning models like LSTM or GRU. While models like Prophet or LSTM work well in specific contexts, ARIMA/SARIMA provide a reliable and efficient baseline for time series forecasting, especially when seasonality and trend components are present.

   

## 🎯 Project Goals
- Forecast **NVIDIA (NVDA)** stock closing prices using ARIMA and SARIMA models.
- Compare multi models performance and select the best fit.
- Demonstrate an end-to-end time series analysis workflow:
  - Data retrieval (yahoo finance)
  - Exploratory Data Analysis (EDA)
  - STL - Decomposition & Stationairty tests (ADF)
  - Modeling (ARIMA, SARIMA for Multi p,d,q Parameters)
  - Evaluation ( Ljung box test, AIC, BIC values, RAMSE )
  - Final Prediction of NVIDIA Stock

---

![End to End Flow](End_to_End_Flow.png)


## 📚 Overview

This repository includes a Jupyter Notebook and supporting scripts to:

1. Load and visualize historical NVIDIA stock data using **Yahoo Finance**.
2. Decompose the time series into **trend**, **seasonal**, and **residual** components using STL.
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

###  Step 1: Clone the repo
```bash
git clone https://github.com/your_username/time-series-arima-sarima.git
cd time-series-arima-sarima

###  Step 2: Install dependencies

Make sure you have Python 3.8+ and pip installed. Then run:

```bash
pip install -r requirements.txt

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

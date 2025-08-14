# Stock Volatility Forecasting (R)

**Authors:** Jan Sklenička & Sebastian Černý

This project analyzes and compares the performance of several volatility models in forecasting the **realized volatility** of **Andeavor (ANDV)**. The goal is to assess **in-sample** and **out-of-sample** predictive accuracy using both classical time-series models and modern approaches that incorporate higher-order moments and conditional heteroskedasticity.

---

## Models Implemented
- **AR(1)** and **HAR** models  
- **HAR** variants with **realized semivariance**, **skewness**, and **kurtosis**  
- **GARCH(1,1)** and **Realized GARCH**  
- Forecast evaluation using **MAE**, **MSE**, **Diebold–Mariano tests**, and **Mincer–Zarnowitz regressions**

---

## Methodology
1. **Data Preparation** – Daily returns and realized volatility constructed from high-frequency intraday data.  
2. **Model Estimation** – Fit candidate models on the in-sample period.  
3. **Forecasting** – Produce 1-step-ahead forecasts via **expanding** and **rolling** windows.  
4. **Evaluation** – Compare models statistically and visually across the full forecast horizon.

---

## Technology
- **R**  
  - Packages: `forecast`, `rugarch`, `highfrequency`, `xts`, `zoo`
- Realized measures computed from intraday price data

> **Reproducibility (R)**
> ```r
> install.packages(c("forecast","rugarch","highfrequency","xts","zoo"))
> # Open the main script / notebook and run sections in order:
> # 1) Data prep  2) In-sample fit  3) Forecasts  4) Evaluation
> ```

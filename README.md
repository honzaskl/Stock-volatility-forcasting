This project created by Jan Sklenička and Sebastian Černý analyzes and compares the performance of various volatility models in forecasting the realized volatility of Andeavor (ticker: ANDV). The aim is to assess both in-sample and out-of-sample predictive accuracy using classical and modern approaches that incorporate higher-order moments and conditional heteroskedasticity.

Models Implemented
AR(1) and HAR models

HAR models with realized semivariance, skewness, and kurtosis

GARCH(1,1) and Realized GARCH

Forecast evaluation using MAE, MSE, Diebold–Mariano tests, and Mincer–Zarnowitz regressions

Methodology
Data Preparation – Daily returns and realized volatility from high-frequency intraday data.

Model Estimation – Fit models on the in-sample period.

Forecasting – Expanding and rolling window procedures.

Evaluation – Statistical and visual comparison of forecast accuracy.

Technology
R (packages: forecast, rugarch, highfrequency, xts, zoo)

High-frequency realized measures computed from intraday price data

Relevance

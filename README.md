# Value-at-Risk-Analysis-from-SPY-Returns

This repository implements a one-day-ahead Value-at-Risk (VaR) forecasting framework for SPY returns, with the code and report made public. The project focuses on **linear quantile regression** as the main method and compares its performance against **GARCH-based VaR** and **neural quantile regression** benchmarks. The analysis emphasizes out-of-sample forecasting, proper backtesting, and statistical calibration of tail risk.



## Data

The dataset used consists of daily observations for the SPDR S&P 500 ETF (SPY), including:

- **log_ret**: daily logarithmic returns
- **rv5**: realized volatility constructed from high-frequency intraday data
- **bv**: bipower variation, capturing the continuous component of price variation

All variables are observable at time $t$ and are used to forecast the next-day return $r_{t+1}$. Missing observations are removed prior to estimation.



## Disclaimer

This project is for academic and educational purposes only and does not constitute financial or investment advice.


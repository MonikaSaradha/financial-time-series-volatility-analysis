# Financial Time Series Volatility Analysis (GARCH, VAR, VECM)

## Overview

This project analyzes financial time series data to model volatility, interdependencies, and long-run relationships between economic variables.

The analysis applies econometric techniques such as GARCH for volatility modeling, VAR for multivariate relationships, and VECM for long-run equilibrium analysis.

This project demonstrates an end-to-end econometric pipeline for analyzing volatility and inter-market relationships in financial time series.

---

## Dataset

The dataset consists of daily financial time series data collected using the `yfinance` API. The analysis focuses on three key market indicators:

* **Crude Oil Prices (CL=F)** – representing global energy market dynamics
* **Exchange Rate (EURUSD=X)** – capturing currency fluctuations between Euro and US Dollar
* **Dow Jones Industrial Average (^DJI)** – reflecting overall stock market performance

The data spans from **January 2020 to July 2023**, with each observation representing adjusted closing prices.

For reproducibility, the dataset is optionally stored locally as `financial_data.xlsx`.

---

## Problem Statement

Financial markets are characterized by:

* volatility clustering
* interdependence between variables
* long-run equilibrium relationships

Understanding these dynamics is critical for risk management, forecasting, and economic analysis.

---

## Objectives

* Analyze volatility patterns in financial time series
* Model time-varying variance using GARCH
* Examine relationships between multiple variables using VAR
* Identify long-run equilibrium using cointegration and VECM

---

## Data Preprocessing

* Retrieved financial data using `yfinance`
* Converted price series to returns
* Checked for stationarity
* Cleaned and structured time series data

---

## Volatility Modeling (GARCH)

* Applied GARCH models to capture volatility clustering
* Forecasted conditional volatility for future periods
* Validated presence of ARCH/GARCH effects using Ljung-Box test

---

## Multivariate Analysis (VAR)

* Built VAR models to analyze interdependence between variables
* Examined lag relationships across oil prices, exchange rates, and stock index
* Generated short-term forecasts

---

## Cointegration & VECM

* Tested for cointegration among variables
* Modeled long-run equilibrium relationships using VECM
* Analyzed adjustment dynamics after short-term shocks

---

## Key Insights

* Strong volatility clustering observed in financial returns
* Oil prices, exchange rates, and stock market are interdependent
* Long-run equilibrium relationships exist between variables
* GARCH effectively captures time-varying volatility

---

## Limitations

* Model sensitivity to lag selection
* External macroeconomic shocks not explicitly modeled
* Limited to historical financial data

---

## Future Improvements

* Extend to multivariate GARCH models
* Include macroeconomic indicators
* Compare with machine learning approaches

---

## Tech Stack

* Python (pandas, numpy, matplotlib)
* yfinance (data collection)
* arch (GARCH modeling)
* statsmodels (VAR, VECM, statistical tests)

---

## Project Structure

* analysis.ipynb – volatility modeling, VAR, and VECM analysis
* README.md – project overview
* project_report.pdf – detailed academic report (supporting material)

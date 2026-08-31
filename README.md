# Financial Data Analysis
### A quantitative research project for portfolio risk analysis and factor investing

---

## Overview and Research Objectives

This project analyzes the return behavior of major US equities, measures tail risk, and backtests systematic portfolio construction strategies against a passive SPY benchmark.

**Assets:** AAPL, MSFT, NVDA, META, GOOGL, SPY  
**Period:** 2020-01-01 to 2025-12-31 (1,506 trading days)

Current objectives include:

- Analyze return distributions of major US equities
- Measure portfolio and asset tail risk
- Build reusable financial data pipelines
- Develop production-quality research code

Long-term objectives:

- Multi-factor investing
- Factor validation
- Portfolio optimization

---

## Features

### Data Pipeline

- Automatic historical data download
- Data cleaning
- Missing value handling
- Reproducible datasets
  
### Statistical Analysis

- Daily and annualized returns, annualized volatility, Sharpe ratio (risk_free_rate = 4.5%)  
- Covariance and correlation matrices
- One-sample and two-sample t-tests on mean daily returns

### Distribution and Risk Analytics

- Distribution visualization, skewness, kurtosis
- Q-Q plots
- Shapiro-Wilk normality testing
- Historical Value-at-Risk (VaR)
- Conditional Value-at-Risk (CVaR)
- Maximum Drawdown

### Portfolio Construction

- Interactive portfolio calculator
- Efficient frontier via 10,000-times Monte Carlo simulations (Dirichlet-sampled weights); identifies Max Sharpe and Min Volatility portfolios
- Backtests three monthly-rebalanced strategies against SPY: equal-weight, momentum-weight (negative-momentum assets get zero weight), and volatility-inverse weight
- Reports annualized return, volatility, Sharpe, max drawdown, and win rate per strategy


## Project Structure

  01_data_acquisition.ipynb 
  
  02_descriptive_statistics.ipynb 
  
  03_distribution_and_tail_risk.ipynb 

  04_portfolio_construction.ipynb
  

## Methodology

The project follows the following research pipeline:

Raw Market Data --> Data Cleaning --> Return Calculation -->  Exploratory Analysis  -->  Distribution Testing  -->  Risk Analysis  -->  Portfolio Analysis

## How to Run

Install dependencies:

pip install pandas numpy matplotlib seaborn scipy yfinance ipywidgets jupyter

Then run notebooks in order (01 → 04) — each depends on data/prices_clean.csv produced by notebook 01:

jupyter notebook

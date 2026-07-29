# Financial Data Analysis
### A quantitative research project for portfolio risk analysis and factor investing

---

## Overview and Research Objectives

The goal of this project is to understand **how financial data behaves**, evaluate **risk**, and build reusable research pipelines.

Current objectives include:

- Analyze return distributions of major US equities
- Measure portfolio and asset tail risk
- Build reusable financial data pipelines
- Develop production-quality research code

Long-term objectives:

- Multi-factor investing
- Factor validation (Fama-MacBeth)
- Portfolio optimization
- Backtesting framework

---

## Features

### Data Pipeline

- Automatic historical data download
- Data cleaning
- Missing value handling
- Reproducible datasets

Assets currently include: SPY, AAPL, MSFT, NVDA, META, GOOGL
  
### Statistical Analysis

- Daily returns
- Annualized returns
- Volatility
- Rolling volatility
- Moving averages
- Distribution visualization
- Q-Q plots
- Skewness
- Kurtosis
- Shapiro-Wilk normality testing

### Risk Analytics

Implemented risk metrics include:

- Historical Value-at-Risk (VaR)
- Conditional Value-at-Risk (CVaR)
- Maximum Drawdown
- Rolling volatility
- Cumulative returns

### Portfolio Construciton

- Construct equal-weight portfolios from selected assets
- Compute daily and cumulative portfolio returns
- Compare portfolio performance against individual assets
- Calculate annualized portfolio return and volatility
- Measure portfolio Maximum Drawdown (MDD)
- Visualize wealth index growth over time
- Evaluate diversification effects through portfolio risk reduction

## Project Structure

  01_data_acquisition.ipynb 
  
  02_descriptive_statistics.ipynb 
  
  03_distribution_and_tail_risk.ipynb 

  04_portfolio_construction.ipynb
  

## Methodology

The project follows the following research pipeline:

Raw Market Data --> Data Cleaning --> Return Calculation -->  Exploratory Analysis  -->  Distribution Testing  -->  Risk Measurement  -->  Portfolio Analysis  -->  Factor Validation

## How to Run

pip install -r requirements.txt

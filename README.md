# Financial Data Analysis

Exploratory analysis of US tech stocks (AAPL, MSFT, NVDA, META, GOOGL) and SPY benchmark. Built to practice using NumPy, pandas, and matplotlib and develop intuition for risk-adjusted returns before moving into strategy backtesting.


## Key Findings

- NVDA delivered the highest return over the period but carried 2.6x the volatility of SPY
- 
- 


## Project Structur

  01_data_acquisition.ipynb 
  
  02_statistical_analysis.ipynb 
  
  03_portfolio_simulator.ipynb 
  

## Methods

- Data: yfinance, daily prices 2020–2025
- Metrics: daily return, 20-day rolling volatility, 50/200-day Moving Average
- Portfolio evaluation: weighted return, portfolio variance, Sharpe Ratio
  (risk-free rate = 4.5%, approximate 2024 T-bill rate)
- Momentum strategy: rank by trailing 12-month return, rebalance monthly


## How to Run

pip install -r requirements.txt

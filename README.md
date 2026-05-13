# Financial Data Analysis

Exploratory analysis of US tech stocks (AAPL, MSFT, NVDA, META, GOOGL) and SPY benchmark. Built to practice using NumPy, pandas, and matplotlib and as a revision for COMM 191 and COMM 298.
The project was developed as a foundation for later work in stochastic modelling and backtesting systems.


## Key Findings

- NVDA delivered the highest return over the period but carried 2.6x the volatility of SPY
- Returns are not normally distributed. Shapiro-Wilk test rejected normality for all tickers (p < 0.05); QQ plots confirm fat tails. Risk models assuming normality will systematically underestimate extreme events
- Momentum strategy outperformed SPY by 23.5% annually, meaning that momentum-based portfolio allocation outperformed equal-weight, but at the cost of 2x the volatility and -41.9% max drawdown vs SPY's -24.5%.


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

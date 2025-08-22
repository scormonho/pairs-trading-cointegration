# Pairs Trading with Cointegration

## 📌 Project Overview
This project demonstrates **pairs trading using cointegration analysis**, a common statistical arbitrage strategy. 
The notebook walks through identifying cointegrated pairs of assets, testing the relationship and implementing 
a simple trading strategy based on mean reversion.

Pairs trading exploits the statistical relationship between two (or more) securities that historically move together. 
When their price ratio diverges beyond a threshold, a long/short position is initiated in expectation of convergence.

---

## ⚙️ Features
- Import and process financial time series data  
- Test for **stationarity** and **cointegration** 
- Identify cointegrated stock pairs  
- Build a trading strategy based on z-score deviations  
- Visualize spreads, z-scores and trading signals  
- Evaluate performance through backtesting  

---

## 📊 Methodology
- Data Collection – Pulls historical stock price data.
- Cointegration Testing – Uses statistical tests to confirm a long-term relationship.
- Spread & Z-Score Calculation – Measures deviation from equilibrium.
- Trading Rules: 
  - Go long the spread when z-score < -1
  - Go short the spread when z-score > +1
  - Exit when spread reverts to the mean (-0.75 < z-score < 0.75)
- Backtest & Visualization – Assess profitability and risk.

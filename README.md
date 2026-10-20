# S&P 500 Moving Average Strategy & Transaction Cost Analysis

## About This Project
I developed this project to test a widely discussed concept empirically: the "Golden Cross" (50/200-day moving average crossover). To efficiently implement this research, I utilized AI-assisted coding tools to build the basic Python framework for data scraping. Yet, the core research design and analysis were driven by curiosity and my own exploration.

## What I Did
1. Extracted 5 years of historical data for the S&P 500 index (`^GSPC`).
2. Simulated a trading rule: Buy when the 50-day moving average crosses above the 200-day moving average (SMA50 > SMA200); Sell when it crosses below.
3. **My Analytical Focus**: Introduced a 0.1% transaction cost per trade to simulate real-world market friction.

## My Findings (The Surprise)
- **SMA Strategy Return (No Costs):** 60.49%
- **SMA Strategy Return (With 0.1% Costs):** 60.01%
- **Simple Buy & Hold Return:** **69.54%**
- **Total Trades Executed:** Only 3

## What I Learned
Because this is a strategy with ultra-low frequency (only 3 trades in 5 years), the transaction cost was negligible (only eroding 0.48%). **The real loss wasn't the trading cost, but the time for "waiting."** The algorithm had to wait for the crossover signals; therefore, it missed the biggest upward rallies in the market. Conversely, a simple Buy-and-Hold approach beat the strategy by over 9 percentage points.

This project taught me a significant lesson in finance and data science: in a highly efficient market, trying to predict the market often fails. As a student determined to pursue Econ and Math, I am eager to continue exploring how market friction and human behavior affect theoretical models in the real world.

## Repository Files
- `S&P500_Backtest_Result.png`: The visualization chart comparing the strategies.
- `main.ipynb`: The Python code used for the backtest.

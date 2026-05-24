# Pairs Trading — Statistical Arbitrage on NSE

A Python implementation of a pairs trading strategy on 17 large-cap NSE stocks (2020–2021).

## What it does
- Fetches 1 year of historical data for 17 Nifty 50 stocks via `yfinance`
- Builds a correlation heatmap to identify highly correlated pairs
- Runs **Engle-Granger cointegration** and **ADF stationarity tests** to find valid pairs
- Identified **Reliance–Infosys** as a cointegrated pair
- Generates **z-score-based buy/sell signals** (entry at ±1, exit at 0)

## Tech Stack
`Python` `Pandas` `Statsmodels` `Matplotlib` `Seaborn` `yFinance`

## Setup
```bash
pip install yfinance pandas statsmodels matplotlib seaborn
jupyter notebook "Pairs Trading.ipynb"
```

## Author
**Debojeet Das** — [LinkedIn](https://linkedin.com/in/debojeetdas)

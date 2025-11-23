
# Stock Analysis & Quantitative Financial Analysis

## Overview

This repository contains notebooks and code for analyzing stock data of six major companies:

- AAPL (Apple Inc.)
- AMZN (Amazon.com Inc.)
- GOOG (Alphabet Inc.)
- META (Meta Platforms, Inc.)
- MSFT (Microsoft Corporation)
- NVDA (NVIDIA Corporation)

The project performs both **descriptive analysis** and **quantitative financial analysis** using Python libraries including `yfinance`, `pandas`, `matplotlib`, `TA-Lib`, and `PyNance`.

---

## Structure



## Features

### 1. Stock Data Collection
- Historical stock data is fetched from Yahoo Finance using the `yfinance` library.
- Columns include **Open, High, Low, Close, Volume**.
- Daily and cumulative returns are calculated for each stock.

### 2. Technical Analysis
- Moving averages (SMA 20, SMA 50) are calculated.
- RSI (Relative Strength Index) identifies overbought/oversold conditions.
- MACD (Moving Average Convergence Divergence) evaluates trend and momentum.

### 3. Portfolio Analysis
- Uses `PyNance` to calculate:
  - **Max Sharpe Ratio Portfolio**
  - **Minimum Variance Portfolio**
  - Efficient frontier visualization

### 4. Visualization
- Price, volume, daily returns, cumulative returns, and technical indicators are plotted for each stock.
- Helps identify trends, volatility, and investment insights.

---

## Usage

1. Open the notebooks in Jupyter Notebook or JupyterLab.  
2. Install the required libraries:

```bash
pip install yfinance pandas matplotlib TA-Lib pynance

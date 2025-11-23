## 📔 Notebooks Readme: Exploratory Data Analysis (EDA)

This directory (`notebooks/`) contains the Jupyter Notebooks used for the **Exploratory Data Analysis (EDA)** of the news article dataset. These notebooks serve as the primary workspace for initial data understanding, visualization, and hypothesis generation.

The analysis is structured to address the core requirements of Task 1, focusing on key attributes like publication time, source, and content characteristics.

---

### 📝 Notebooks Overview

| Filename | Focus Area | Description | Status |
| :--- | :--- | :--- | :--- |
| `01_descriptive_stats.ipynb` | **Descriptive Statistics** | Calculates and visualizes basic metrics: text length distributions (e.g., headline/body), and raw counts of articles. | In Progress |
| `02_publisher_analysis.ipynb` | **Publisher and Source** | Focuses on **publisher-specific analysis**: counting articles per source, identifying unique domains, and comparing activity levels. | In Progress |
| `03_time_series_eda.ipynb` | **Time Series Analysis** | Investigates publication date/time trends: frequency over time (daily, hourly), identifying spikes, and analyzing **publishing times** for market relevance. | To Do |
| `04_text_topic_modeling.ipynb` | **Text/NLP Analysis** | Performs preliminary text processing and visualization (e.g., word clouds, common n-grams) to uncover initial themes and keywords. | To Do |

---

### 🔍 Key Areas of Raw Analysis

The notebooks aim to answer fundamental questions about the dataset, which are crucial for any downstream modeling:

#### 1. Publisher Raw Analysis
* **Most Active Publishers:** Which publishers contribute the highest volume of news?
* **Domain Identification:** If publishers are email addresses, identification and frequency analysis of unique organizational domains.
* **Volume Distribution:** Visualization of the article count distribution across all unique publishers (e.g., Pareto Chart).

#### 2. Publication Time Analysis
* **Frequency Over Time:** Time-series plots showing the total volume of articles published daily or hourly.
* **Event Spikes:** Identifying and investigating specific dates or time windows with unusually high publication volume, which may correlate with known market events.
* **Intra-Day Patterns:** Analyzing the **hour of the day** when the majority of news is released to detect consistent publishing patterns.

---

### 🛑 Prerequisites and Reproducibility

To run these notebooks, you must have the required Python environment set up as defined in the main project's `requirements.txt`.

1.  **Activate Environment:** Ensure your Python environment is active.
2.  **Kernel Selection:** Select the appropriate Python kernel for these notebooks.
3.  **Data Location:** The notebooks assume the **raw data is accessible** or has been loaded by a script (e.g., in the `scripts/` directory) and is ready for use

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

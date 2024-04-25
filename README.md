Sure, here's a sample README file highlighting the important aspects of the provided code:

---

# Unsupervised Learning Trading Strategy

This repository contains Python code for implementing an unsupervised learning trading strategy using machine learning techniques.

## Overview

The trading strategy aims to:

1. Group similar assets based on their features using K-Means clustering.
2. Select assets for each month based on the cluster and form a portfolio.
3. Optimize the portfolio using Efficient Frontier max sharpe ratio optimization.
4. Calculate daily portfolio returns and compare them to NIFTY500 returns.

## Key Features

### Data Collection and Preprocessing

- **Web Scraping**: Data is scraped from Wikipedia to obtain the list of NIFTY500 stocks.
- **Yahoo Finance API**: Historical stock data is retrieved using Yahoo Finance API.
- **Calculations**: Various finance parameters such as Garman-Klass volatility, RSI, Bollinger Bands, ATR, MACD, and rupees volume are calculated.
- **Aggregation**: Data is aggregated to monthly level and the top 150 most liquid stocks are selected for each month.

### Clustering and Portfolio Optimization

- **K-Means Clustering**: Assets are grouped into clusters based on their features.
- **Portfolio Optimization**: Portfolio weights are optimized using Efficient Frontier max sharpe ratio optimization. If optimization fails, equal weights are applied.

### Performance Evaluation

- **Visualizations**: Portfolio returns are visualized and compared with NIFTY500 returns through time series plots, histograms, cumulative returns plots, and density plots.
- **Metrics**: The highest strategy return throughout the period is calculated for performance evaluation.

## Usage

1. Install the required libraries using `pip install -r requirements.txt`.
2. Run the Python script `trading_strategy.py` to execute the trading strategy.
3. View the generated plots to analyze the performance of the trading strategy.

## Dependencies

- pandas
- numpy
- matplotlib
- statsmodels
- seaborn
- scikit-learn
- yfinance
- pandas_ta
- pypfopt

## Contributors

- [Kavin Puri](https://github.com/kavinpuri)

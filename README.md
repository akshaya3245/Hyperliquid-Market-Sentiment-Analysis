# Hyperliquid-Market-Sentiment-Analysis

## Project Overview

This project investigates how Hyperliquid market sentiment (Fear & Greed Index) influences trader behavior and trading performance on Hyperliquid.

The objective is to identify statistically supported behavioral patterns that can inform better trading strategies.

---

## Dataset

### 1. Market Sentiment Data

- Daily Fear & Greed Index
- Columns:
  - Timestamp
  - Value
  - Classification
  - Date

### 2. Hyperliquid Historical Trader Data

Contains:

- Account
- Coin
- Execution Price
- Size Tokens
- Size USD
- Side
- Timestamp IST
- Start Position
- Direction
- Closed PnL
- Transaction Hash
- Order ID
- Crossed
- Fee
- Trade ID
- Timestamp
  

---

## Project Workflow

1. Data Cleaning
2. Timestamp Standardization
3. Daily Data Alignment
4. Feature Engineering
5. Statistical Analysis
6. Trader Segmentation
7. Strategy Recommendations

---

## Features Created

- Daily PnL per Account
- Win Rate
- Average Trade Size
- Trades per Day
- Long / Short Ratio
- Trader Segments
  - Frequent vs Infrequent
  - Consistent vs Inconsistent Winners
  - Large vs Small Position Traders

---

## Statistical Tests

- Welch's t-test
- Mann–Whitney U Test

---

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook

---

## Installation

```bash
https://github.com/akshaya3245/Hyperliquid-Market-Sentiment-Analysis

cd Hyperliquid-Market-Sentiment-Analysis

pip install -r requirements.txt
```

---

## Run

Open

```
notebooks/Hyperliquid_Market_Sentiment_Analysis.ipynb
```

Run every notebook cell.

---

## Outputs

The notebook generates

- Charts
- Summary tables
- Statistical test results
- Trader segmentation
- Strategy recommendations

---

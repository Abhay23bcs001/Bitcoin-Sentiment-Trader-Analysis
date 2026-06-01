# 📊 Bitcoin Market Sentiment vs Trader Performance Analysis

## Exploring the Relationship Between Bitcoin Market Sentiment and Hyperliquid Trader Performance

### Data Science Hiring Assessment Submission

---

# 📌 Project Overview

Financial markets are heavily influenced by investor psychology and sentiment. Understanding how market sentiment impacts trader behavior can provide valuable insights for designing profitable trading strategies and risk management systems.

This project investigates the relationship between Bitcoin market sentiment and trader performance by combining:

1. **Bitcoin Fear & Greed Index Dataset**
2. **Hyperliquid Historical Trader Dataset**

The objective is to determine whether market sentiment influences:

* Trading profitability
* Win rate
* Trading volume
* Trader behavior
* Market risk and volatility

---

# 🎯 Problem Statement

Analyze the relationship between Bitcoin market sentiment and trader performance using historical trading data and the Fear & Greed Index.

The key questions addressed are:

* Does trader profitability change across different sentiment conditions?
* Which sentiment category generates the highest profits?
* How does trader behavior differ during Fear and Greed periods?
* Can sentiment be used as a useful signal for trading decisions?

---

# 📂 Datasets Used

## Dataset 1: Bitcoin Fear & Greed Index

This dataset represents daily Bitcoin market sentiment.

### Features

| Column         | Description        |
| -------------- | ------------------ |
| timestamp      | Unix timestamp     |
| value          | Sentiment score    |
| classification | Sentiment category |
| date           | Date               |

### Sentiment Categories

* Extreme Fear
* Fear
* Neutral
* Greed
* Extreme Greed

---

## Dataset 2: Hyperliquid Historical Trader Data

This dataset contains detailed trading activity from the Hyperliquid trading platform.

### Features

| Column           | Description                      |
| ---------------- | -------------------------------- |
| account          | Trader wallet address            |
| coin             | Asset traded                     |
| execution price  | Trade execution price            |
| size tokens      | Number of tokens traded          |
| size usd         | Trade size in USD                |
| side             | BUY or SELL                      |
| timestamp        | Trade timestamp                  |
| start position   | Initial position size            |
| direction        | Trade direction                  |
| closed pnl       | Realized profit/loss             |
| transaction hash | Blockchain transaction reference |
| order id         | Trade order identifier           |

---

# 🛠️ Tools and Technologies

### Programming Language

* Python

### Libraries Used

* Pandas
* NumPy
* Matplotlib
* Seaborn

### Environment

* Jupyter Notebook

### Version Control

* Git
* GitHub

---

# 🔄 Project Workflow

## Step 1: Data Loading

Imported both datasets into Pandas DataFrames.

## Step 2: Data Cleaning

Performed:

* Column standardization
* Data type correction
* Missing value inspection

## Step 3: Date Standardization

Converted timestamps into common date format.

## Step 4: Dataset Integration

Merged trader data with sentiment data using date as the common key.

## Step 5: Exploratory Data Analysis

Performed:

* Sentiment analysis
* Profitability analysis
* Volume analysis
* Win rate analysis
* Volatility analysis

## Step 6: Visualization

Generated charts for:

* Profitability
* Win Rate
* Trading Volume
* Volatility
* Correlation Analysis

---

# 📊 Analysis Performed

## 1. Sentiment Distribution Analysis

Examined the frequency of each market sentiment category.

---

## 2. Average Profit/Loss Analysis

Measured average trader profitability across:

* Extreme Fear
* Fear
* Neutral
* Greed
* Extreme Greed

---

## 3. Total Profitability Analysis

Calculated cumulative profits generated under each sentiment condition.

---

## 4. Win Rate Analysis

Determined percentage of profitable trades across sentiment categories.

---

## 5. Buy vs Sell Behavior Analysis

Investigated trader behavior during different market conditions.

---

## 6. Trading Volume Analysis

Measured total trading volume under different sentiment classes.

---

## 7. Volatility Analysis

Analyzed profit variability using standard deviation of Closed PnL.

---

## 8. Correlation Analysis

Studied relationships between:

* Execution Price
* Trade Size
* Position Size
* Profitability

---

# 📈 Key Findings

## Finding 1

### Extreme Greed Produced the Highest Average Profit

Average PnL:

* Extreme Greed → 205.82
* Fear → 128.29
* Greed → 53.99
* Neutral → 27.09
* Extreme Fear → 1.89

---

## Finding 2

### Fear Generated the Highest Total Profit

Total PnL:

* Fear → 1.78 Million
* Extreme Greed → 1.16 Million
* Greed → 0.61 Million
* Neutral → 0.07 Million
* Extreme Fear → 0.004 Million

---

## Finding 3

### Extreme Greed Achieved the Highest Win Rate

Win Rate:

* Extreme Greed → 55.33%
* Neutral → 49.49%
* Greed → 43.57%
* Fear → 38.18%
* Extreme Fear → 29.28%

---

## Finding 4

### Extreme Fear Produced the Weakest Performance

* Lowest average profitability
* Lowest win rate
* Lowest overall trader performance

---

## Finding 5

### Fear Generated the Highest Trading Volume

Trading Volume:

* Fear → 79.67 Million USD
* Greed → 57.05 Million USD
* Extreme Greed → 18.22 Million USD
* Neutral → 11.94 Million USD
* Extreme Fear → 9.58 Million USD

---

## Finding 6

### SELL Orders Dominated During Greed Periods

Traders appeared to lock in profits during:

* Greed
* Extreme Greed

---

## Finding 7

### Extreme Greed Showed Highest Volatility

Profit Volatility:

* Extreme Greed → 1861.56
* Greed → 1399.47
* Fear → 1342.35
* Neutral → 142.95
* Extreme Fear → 76.73

Higher profitability was associated with higher risk.

---

# 📷 Visualizations

The repository contains visualizations for:

* Average PnL by Sentiment
* Total PnL by Sentiment
* Win Rate by Sentiment
* Trading Volume by Sentiment
* Profit Volatility
* Correlation Heatmap

All visualizations are available in the **visuals/** directory.

---

# 💡 Business Insights

The analysis indicates that market sentiment significantly impacts trader behavior and profitability.

Key observations:

* Fear periods generate high market participation and large cumulative profits.
* Extreme Greed periods offer the highest average profitability.
* Extreme Fear is generally unfavorable for trading performance.
* Market sentiment can be used as a supplementary signal for trading decisions.

---

# 🚀 Recommendations

### Recommendation 1

Use sentiment indicators as an additional confirmation signal.

### Recommendation 2

Apply stricter risk management during Extreme Fear periods.

### Recommendation 3

Monitor Extreme Greed carefully because it offers both high profitability and high volatility.

### Recommendation 4

Use sentiment-aware position sizing.

### Recommendation 5

Combine sentiment analysis with technical indicators and market structure analysis.

---

# 📌 Conclusion

This project demonstrates a strong relationship between Bitcoin market sentiment and trader performance.

Key conclusions:

* Extreme Greed generated the highest average profitability and win rate.
* Fear generated the highest total profitability and trading volume.
* Extreme Fear produced the weakest trading outcomes.
* Sentiment-based analysis can improve trading strategies and risk management systems.

The findings suggest that market sentiment should be considered as an important supplementary factor in cryptocurrency trading decisions.

---

# 📁 Repository Structure

```text
Bitcoin-Sentiment-Trader-Analysis

│
├── data
│   ├── fear_greed_index.csv
│   └── historical_data.csv
│
├── notebooks
│   └── analysis.ipynb
│
├── visuals
│   ├── charts
│   └── heatmaps
│
├── report
│   └── Final_Report.pdf
│
└── README.md
```

# 👨‍💻 Author

**Abhay Sharma**

Data Science Hiring Assessment Submission

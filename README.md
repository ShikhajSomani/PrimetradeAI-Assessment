# 📊 Trader Performance vs Market Sentiment Analysis

## 📌 Overview
This project analyzes how market sentiment (Fear vs Greed) impacts trader behavior and performance using Hyperliquid trading data. The objective is to identify patterns in profitability, risk-taking, and trading behavior, and to derive actionable trading strategies based on sentiment conditions.

---

## 📂 Datasets

### 1. Market Sentiment Dataset
- Columns: date, classification (Fear / Greed)

### 2. Trader Dataset (Hyperliquid)
- Columns include:
  - Account
  - Execution Price
  - Size USD
  - Side
  - Closed PnL
  - Timestamp IST
  - Start Position

---

## ⚙️ Setup Instructions

### 1. Clone the repository
git clone <your-repository-link>  
cd <your-repository-name>

### 2. Install required libraries
pip install pandas numpy matplotlib seaborn

### 3. Run the notebook
jupyter notebook

Open the notebook file:
Trader_Sentiment_Analysis.ipynb

---

## 🧠 Methodology

### 🔹 Data Cleaning
- Removed duplicate records  
- Handled missing values  
- Converted timestamp columns to datetime format  

### 🔹 Data Alignment
- Extracted date from trader timestamps (Timestamp IST)  
- Converted sentiment dataset to daily format  
- Merged both datasets using the date column  

### 🔹 Feature Engineering
Created the following key metrics:
- Daily PnL (profit per trader per day)  
- Win Rate (percentage of profitable trades)  
- Trade Count (number of trades per day)  
- Average Trade Size  
- Leverage (proxy)  
- Long/Short Ratio  

### 🔹 Aggregation
- Grouped data by date, Account, and classification  
- Generated daily-level metrics for each trader  

### 🔹 Analysis
- Compared trader performance across Fear vs Greed days  
- Analyzed behavioral changes (leverage, activity, trade size)  
- Performed segmentation:
  - High vs Low leverage traders  
  - Frequent vs Infrequent traders  
  - Consistent vs Inconsistent traders  

---

## 📊 Key Insights

- Traders tend to achieve higher average PnL during Greed periods, indicating favorable market conditions.  
- Leverage usage increases during Greed, reflecting higher risk appetite.  
- High-leverage traders experience larger losses during Fear periods, indicating vulnerability in bearish conditions.  
- Trading activity increases during Greed but becomes unstable during sentiment transitions.  

---

## 💡 Strategy Recommendations

### 🔹 Strategy 1: Risk Reduction During Fear
Reduce leverage and position sizes during Fear periods, especially for high-leverage traders, to minimize losses.

### 🔹 Strategy 2: Controlled Aggression During Greed
Increase trading activity and moderately increase leverage during Greed periods while maintaining risk control.

### 🔹 Strategy 3: Avoid Overtrading
Reduce trade frequency during transitions between Fear and Greed to avoid unnecessary losses.

---

## 📈 Outputs

The notebook includes:
- Bar charts comparing PnL and leverage across sentiment  
- Distribution plots (PnL variability)  
- Segmentation tables (leverage groups, activity levels)  

---

## 🚀 Conclusion

Market sentiment has a significant impact on trader performance and behavior. Adapting trading strategies based on sentiment conditions can improve profitability while effectively managing risk.

---

## 📎 Files Included

- assessment.ipynb → Main notebook  
- README.md → Project documentation  

---

## 👨‍💻 Author

SHIKHAJ SOMANI
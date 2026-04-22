
---

# 📄 2. Short Write-up (1-page summary)

```markdown
# 📊 Trader Performance vs Market Sentiment — Summary

## 🔍 Objective
The objective of this analysis is to study how market sentiment (Fear vs Greed) influences trader behavior and performance on Hyperliquid.

---

## ⚙️ Methodology

The analysis began with cleaning and preprocessing two datasets: trader activity data and market sentiment data. Timestamps from the trader dataset were converted to daily format and aligned with sentiment data using date.

Key metrics were engineered at a daily level per trader, including:
- Daily PnL
- Win rate
- Trade frequency
- Average trade size
- Leverage proxy
- Long/Short ratio

The data was then aggregated and analyzed across sentiment categories (Fear vs Greed). Additional segmentation was performed to evaluate differences across trader types (e.g., high vs low leverage, frequent vs infrequent traders).

---

## 📊 Key Insights

1. Traders tend to generate higher average profits during Greed periods, likely due to increased market momentum and confidence.

2. Leverage usage is significantly higher during Greed days, indicating a stronger risk appetite among traders.

3. High-leverage traders are more vulnerable during Fear periods, experiencing larger losses and higher volatility.

4. Trading activity increases during Greed but becomes less stable during sentiment transitions, leading to inconsistent performance.

---

## 💡 Strategy Recommendations

1. **Risk Control in Fear Markets:**  
   Reduce leverage and trade size during Fear periods to minimize downside risk.

2. **Capitalizing on Greed Markets:**  
   Increase trade participation and moderately increase leverage during Greed periods while maintaining risk discipline.

3. **Avoid Overtrading:**  
   Reduce trading frequency during sentiment transitions to avoid unnecessary losses.

---

## 🚀 Conclusion

The analysis demonstrates that market sentiment plays a critical role in shaping trader behavior and performance. By adapting trading strategies based on sentiment conditions, traders can improve profitability while effectively managing risk.
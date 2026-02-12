# Trader Performance vs Market Sentiment Analysis

## 📌 Objective

This project analyzes how Bitcoin market sentiment (Fear / Greed Index) impacts trader behavior and performance on Hyperliquid.

The goal is to identify patterns in profitability, risk-taking behavior, and trading frequency under different sentiment regimes and propose actionable trading strategies.

---

## 📊 Datasets Used

1. **Bitcoin Market Sentiment Dataset**
   - Columns: timestamp, value, classification, date
   - Contains daily Fear/Greed classification.

2. **Historical Trader Data (Hyperliquid)**
   - Columns include: Account, Timestamp IST, Closed PnL, Size USD, Side, Fee, etc.
   - Contains detailed trade-level data.

---

## 🛠 Methodology

### 1️⃣ Data Preparation
- Removed duplicates and checked missing values.
- Converted timestamps to daily format.
- Merged trader data with sentiment data on Date.
- Created engineered features:
  - Daily PnL per trader
  - Win rate
  - Average trade size
  - Trade frequency
  - Long/Short ratio

### 2️⃣ Sentiment-Based Analysis
- Compared average PnL across sentiment categories.
- Analyzed trade frequency during Fear vs Greed.
- Examined position size changes.
- Evaluated win rate and volatility differences.

### 3️⃣ Trader Segmentation
- Frequent vs Infrequent traders
- Consistent vs Inconsistent traders
- Risk-based behavior analysis

---

## 📈 Key Findings

1. **Greed periods generate the highest average PnL.**
2. **Trading activity peaks during Fear periods.**
3. **Position sizes significantly increase during Greed, indicating higher risk appetite.**
4. Performance declines during Extreme Greed, suggesting overconfidence effects.
5. Fear periods show increased activity but smaller capital deployment.

---

## 💡 Strategy Recommendations

1. Increase exposure cautiously during Greed periods.
2. Avoid over-leveraging during Extreme Greed.
3. Monitor high-frequency trading activity during Fear for volatility opportunities.
4. Implement dynamic risk management based on sentiment conditions.

---

## 📊 Visualizations Included

- Average PnL by Sentiment
- Trade Size Comparison by Sentiment
- Win Rate by Sentiment
- PnL Distribution Boxplots

---

## 🧰 Tools Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib

---

## ▶ How to Run

1. Clone the repository:
git clone <your_repo_link>


2. Install dependencies:
pip install -r requirements.txt


3. Open the notebook:
jupyter notebook trader_sentiment_analysis.ipynb


---

## 📌 Conclusion

Market sentiment significantly influences trader behavior. 
Greed increases risk-taking and profitability, while Fear increases trading activity but with more cautious capital allocation.

Understanding sentiment-driven behavior can help design adaptive trading strategies.
# Trader Behavior vs Bitcoin Market Sentiment

## Overview
This project analyzes the relationship between Bitcoin market sentiment
(Fear & Greed Index) and trader behavior using historical trade data.

The objective is to understand how emotional market conditions influence
trader performance, risk-taking behavior, and trading activity, and to
derive insights that can support smarter trading and risk management strategies.

---

## Datasets Used

1. **Bitcoin Fear & Greed Index**
   - Daily market sentiment classification (Fear, Neutral, Greed)
   - Includes sentiment intensity score (0–100)

2. **Historical Trader Data**
   - Executed Bitcoin trades
   - Includes position size, trade direction, and realized PnL

Both datasets are merged at a daily level to align market sentiment
with actual trading behavior.

---

## Methodology

The analysis follows a structured data science workflow:

1. Data loading and initial inspection
2. Data cleaning and preprocessing
3. Feature engineering
   - Profit/loss flags
   - Risk proxy using position size
4. Data integration using daily sentiment alignment
5. Exploratory Data Analysis (EDA) using distribution-based
   and multi-metric visualizations
6. Insight generation and business interpretation

Visualization scales were selected using percentile-based limits
and log transformations to avoid distortion from extreme outliers.

---

## Key Analyses

- **Profitability Distribution Analysis**  
  Examined how profit and loss distributions vary across sentiment regimes.

- **Trading Activity vs Performance**  
  Compared trade frequency with win rates to identify overtrading behavior.

- **Risk-Taking Behavior**  
  Analyzed position size distributions as a proxy for trader risk appetite.

- **Loss Severity Analysis**  
  Evaluated downside risk during different market sentiment phases.

- **Risk vs Outcome Relationship**  
  Explored the relationship between risk exposure and trade outcomes
  using scatter plots with trend analysis.

---

## Key Findings

- Greed-driven markets show wider PnL distributions and heavier downside risk.
- Trading activity increases during Greed phases, while win rates decline.
- Traders take larger position sizes during positive sentiment, indicating overconfidence.
- Losses are more severe during Greed periods compared to Fear-driven markets.
- Higher risk exposure does not consistently lead to better outcomes.

---

## Business Implications

The findings suggest that market sentiment plays a critical role in shaping
trader behavior and performance.

Incorporating sentiment-aware risk controls—such as limiting position sizes
and controlling trade frequency during Greed phases—can help reduce downside
risk and improve overall trading performance.

Market sentiment can therefore serve as a valuable input for designing
behavior-aware trading strategies and risk management frameworks.

---

## How to Run the Project

1. Clone or download the repository
2. Install dependencies:
```bash
pip install -r requirements.txt


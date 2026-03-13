# trader-sentiment-analysis
"An end-to-end quantitative analysis exploring how macroeconomic sentiment (Fear &amp; Greed Index) impacts trader behavior, leverage, and profitability on Hyperliquid."

# 📈 Trader Performance vs. Market Sentiment Analysis

**Candidate:** Nitish Patel  
**Role:** Data Science Intern Candidate  
**Target:** Primetrade.ai / Anything.ai  

## 🎯 Project Objective
This project explores the intersection of macroeconomic psychology and micro-level quantitative execution. By merging the **Bitcoin Fear & Greed Index** with over 210,000 historical trade logs from the **Hyperliquid** platform, this analysis aims to uncover behavioral inefficiencies—such as FOMO, revenge trading, and risk expansion—and translate them into systematic trading rules.

## 📂 Repository Structure
* `trader_behavior_analysis.ipynb` - The primary Jupyter Notebook containing the complete Python workflow (Data Cleaning, EDA, Segmentation, Machine Learning).
* `/charts/` - Contains all exported high-resolution visualizations used in the analysis.
* `/data/` - *(Ignored via .gitignore)* Local directory for the raw `fear_greed_index.csv` and `historical_data.csv` datasets.
* `requirements.txt` - Python dependencies required to reproduce the environment.

## ⚙️ Methodology & Reproducibility
The analysis follows a strict end-to-end data science lifecycle:
1. **Data Alignment & Cleaning:** Normalized timestamps across diverse datasets to perform daily temporal alignment. Handled missing margin data by establishing synthetic risk proxies to demonstrate quantitative workflows.
2. **Feature Engineering:** Developed custom trader KPIs, including *Daily PnL*, *Trade Frequency*, *Average Trade Size*, *Long/Short Ratio*, and *Average Leverage*.
3. **Behavioral Cohort Analysis:** Segmented traders using statistical medians (e.g., High vs. Low Leverage, Consistent Winners vs. Inconsistent Traders) to isolate systemic edge.
4. **Predictive Machine Learning:** Deployed a `RandomForestClassifier` to predict daily profitability based purely on execution mechanics and market sentiment.

### Quick Start
To reproduce this environment locally, run the following commands in your terminal:

```bash
git clone [https://github.com/nitishpatel19/trader-sentiment-analysis.git](https://github.com/nitishpatel19/trader-sentiment-analysis.git)
cd trader-sentiment-analysis
pip install -r requirements.txt
jupyter notebook trader_behavior_analysis.ipynb

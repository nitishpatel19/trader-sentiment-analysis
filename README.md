# trader-sentiment-analysis
"An end-to-end quantitative analysis exploring how macroeconomic sentiment (Fear &amp; Greed Index) impacts trader behavior, leverage, and profitability on Hyperliquid."

# 📈 Trader Performance vs. Market Sentiment Analysis

**Candidate:** Nitish Patel  
**Role:** Junior Data Scientist Candidate  
**Target Team:** Primetrade.ai / Anything.ai  
**Live Dashboard:** [View Interactive Analytics](https://trader-sentiment-analysis-liygpgx6ybudqn5btq4uca.streamlit.app/)

## 🎯 Project Objective
This project explores the intersection of macroeconomic psychology and micro-level quantitative execution. By merging the **Bitcoin Fear & Greed Index** with over 210,000 historical trade logs from the **Hyperliquid** platform, this analysis aims to uncover behavioral inefficiencies—such as FOMO, revenge trading, and risk expansion—and translate them into systematic trading rules.

## 📂 Repository Structure
* `app.py` - Production code for the live Streamlit dashboard.
* `trader_behavior_analysis.ipynb` - Comprehensive research notebook including Data Cleaning, EDA, and Machine Learning.
* `requirements.txt` - Dependency list for reproducing the environment.
* `Data/` - Contains the processed datasets used for analysis and the dashboard.
* `charts/` - High-resolution visualizations exported from the analysis.

## ⚙️ Methodology & Reproducibility
The analysis follows a strict end-to-end data science lifecycle:
1. **Data Alignment:** Normalized diverse temporal datasets to perform daily alignment between execution logs and sentiment scores.
2. **Feature Engineering:** Developed custom trader KPIs: *Daily PnL*, *Trade Frequency*, *Long/Short Ratio*, and *Average Leverage*.
3. **Behavioral Archetyping:** Used **K-Means Clustering** to segment traders into distinct archetypes based on risk profile and execution consistency.
4. **Predictive Modeling:** Deployed a **RandomForestClassifier** to determine the probability of a profitable session based on market sentiment and historical execution mechanics.

### Quick Start (Local Setup)
```bash
git clone [https://github.com/nitishpatel19/trader-sentiment-analysis.git](https://github.com/nitishpatel19/trader-sentiment-analysis.git)
cd trader-sentiment-analysis
pip install -r requirements.txt
streamlit run app.py

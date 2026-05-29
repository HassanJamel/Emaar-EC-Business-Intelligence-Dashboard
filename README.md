<p align="center">
  <a href="https://www.kaggle.com/code/hassanjameelahmed/emaar-ec-business-intelligence-dashboard" target="_blank">
    <img src="Emaar Historical Analysis.jpg" alt="Emaar Historical" alt="Emaar Historical" width="600">
  </a>
</p>
<br>




# Emaar The Economic City (Tadawul: 4220) Historical Stock Data Analysis

## SEO-Optimized Project Name and Description
**Project Name:** Emaar The Economic City (Tadawul: 4220) Historical Stock Market Dataset
**Description:** Dive into over a decade of historical financial data for Emaar The Economic City, a leading real estate and master development company in Saudi Arabia. This dataset features daily stock prices, including open, high, low, close, and trading volume, essential for time series forecasting, algorithmic trading, and economic research.

## Top 5 Kaggle Tags
1. Finance
2. Stock Market
3. Real Estate
4. Saudi Arabia
5. Time Series Analysis

## Dataset Details
This dataset contains historical daily trading data for Emaar The Economic City. 

**Columns Information:**
- **Date:** The trading date (Format: MM/DD/YYYY).
- **Close:** The closing price of the stock on the given trading day.
- **High:** The highest price of the stock reached during the trading session.
- **Low:** The lowest price of the stock reached during the trading session.
- **Open:** The opening price of the stock at the beginning of the trading session.
- **Volume:** The total number of shares traded during the session.

## Coverage
- **Temporal Scope:** The dataset covers daily trading records starting from **03/04/2010** to **01/29/2026**.
- **Geospatial Scope:** Kingdom of Saudi Arabia (Saudi Exchange - Tadawul).

## Data Provenance & Source
**Provenance:** The data is sourced directly from historical market records of the Saudi Exchange (Tadawul) and related financial data aggregators. The raw data is aggregated and maintained to reflect daily stock movements without synthetic alterations, ensuring high fidelity for financial and quantitative analysis.
**Correct Source:** Tadawul (Saudi Exchange)
**Source Link:** [Saudi Exchange - Emaar The Economic City (4220)](https://www.saudiexchange.sa/wps/portal/tadawul/home/)

## Dataset Collecting Methodology
The dataset is collected through automated extraction of historical daily trading summaries from financial data APIs or the official Saudi Exchange portals. The collection methodology involves capturing end-of-day trading metrics (Open, High, Low, Close, Volume) and formatting them into a structured CSV file for ease of use in predictive modeling, technical analysis, and exploratory data analysis.

## Biggest Problems and Challenges Facing This Project
1. **Market Gaps & Holidays:** The Saudi Exchange operates on a Sunday-Thursday schedule, and observing public holidays creates non-linear gaps in the time-series data that require handling before running continuous forecasting models.
2. **Data Adjustments:** Historical stock prices may need adjustments for corporate actions such as stock splits, dividends, or capital reductions to maintain analytical accuracy. If the data is unadjusted, sudden price drops might falsely appear as market crashes.
3. **Volatility Modeling:** Real estate and mega-development projects (like King Abdullah Economic City) are highly sensitive to macro-economic factors (e.g., oil prices, interest rates). Isolating the stock's performance from broader market noise is a significant challenge.
4. **Predictive Accuracy:** Building robust machine learning models to accurately forecast future stock movements based purely on historical OHLCV data is notoriously difficult due to the efficient market hypothesis and exogenous market shocks.

## Problem Development (Step-by-Step)
1. **Initial Objective Definition:** The project begins with a need to understand the financial trajectory and market valuation of Emaar The Economic City, a key player in Saudi Arabia's mega-projects and real estate sector.
2. **Data Identification & Acquisition:** Historical stock data (OHLCV) was identified as the primary quantifiable metric to assess investor sentiment and company performance over time. The data spanning from early 2010 to early 2026 was extracted and compiled.
3. **Data Preprocessing & Cleaning:** Initial inspection of the data reveals the need to format the `Date` column into a standard datetime object, sort the records chronologically, and verify the absence of null values or anomalous zero-volume days. Missing days due to weekends and holidays must be appropriately handled (e.g., forward-filling or using business day frequencies).
4. **Exploratory Data Analysis (EDA):** The next step involves plotting the Closing price over time to visualize macroeconomic trends, calculating moving averages (e.g., 50-day, 200-day) to identify bullish/bearish trends, and analyzing volume spikes corresponding to major corporate announcements.
5. **Feature Engineering:** Developing the problem further requires creating technical indicators (RSI, MACD, Bollinger Bands) from the raw data to provide predictive signals to machine learning models.
6. **Model Building & Forecasting:** Finally, applying time-series forecasting algorithms (like ARIMA, Prophet, or Recurrent Neural Networks/LSTMs) to predict future price movements based on historical patterns, while acknowledging the inherent challenges and volatility of the real estate sector.

# Energy Market Spread Analysis (2015–2025)

## Overview

This project analyzes the behavior and interrelationships of global energy markets over a 10-year period (January 2015 – January 2025) using weekly closing price data.

The focus is on crude oil, natural gas, LNG, and selected refined products, using both spot and futures prices where available. The goal is to understand how these markets move relative to each other, identify structural relationships, and evaluate the behavior of key energy spreads.

---

## Objectives

- Analyze long-term price behavior across major energy commodities  
- Identify relationships between crude oil, natural gas, LNG, and refined products  
- Examine key spreads such as Brent–WTI and refining crack spreads  
- Study volatility patterns and market regimes  
- Evaluate risk-adjusted performance of spreads  
- Understand structural dynamics in global energy markets  

---

## Data Sources

- Investing.com  
- Yahoo Finance  
- Federal Reserve Economic Data (FRED)  

The dataset consists of weekly closing prices from January 2015 to January 2025.  
Daily data (where applicable) was resampled to weekly frequency for consistency across assets.

---

## Data Preprocessing

- Converted all datasets to a common weekly frequency  
- Handled missing values using:
  - Time-based linear interpolation  
  - ARIMA-based interpolation for more complex gaps  
- Removed assets with excessive missing or sparse observations  
- Aligned all time series for comparative analysis  

---

## Methodology

### Exploratory Data Analysis (EDA)
- Price trend analysis  
- Weekly returns  
- Rolling volatility  
- Seasonality patterns  

### Correlation & Regression Analysis
- Correlation matrix across energy assets  
- Multicollinearity checks using Variance Inflation Factor (VIF)  
- Multiple linear regression to explore relationships between variables  

### Spread Analysis
- Brent–WTI spread  
- Crack spreads (e.g., gasoline, 3-2-1 refining spreads)  
- Analysis of structural vs. short-term spread behavior  

### Risk & Performance Analysis
- Volatility clustering  
- Fat-tail behavior and asymmetric risk  
- Sharpe ratios and risk-adjusted performance  

---

## Key Insights

- Energy spreads reflect **structural market differences**, not just short-term price movements  
- The Brent–WTI spread captures long-standing regional segmentation between global seaborne markets and U.S. inland supply  
- Volatility is **state-dependent**, clustering during periods of stress such as geopolitical events and supply disruptions  
- Refining spreads exhibit **asymmetric downside risk**, with larger and faster negative movements compared to positive ones  
- Risk-adjusted performance varies significantly across spreads:
  - Brent–WTI shows weak or negative Sharpe ratios  
  - Crack spreads show modest but relatively more consistent performance  

Overall, energy spread trading is best approached as a **risk-managed and timing-sensitive strategy**, rather than a purely directional investment.

---

## Conclusions

- Energy markets are highly interconnected across commodities and regions  
- Relative pricing (spreads) provides deeper insights than outright price levels  
- Volatility and risk are dynamic and should be treated as regime-dependent  
- Structural factors such as infrastructure, supply constraints, and demand shifts play a major role in spread behavior  

This analysis highlights the importance of viewing energy markets through a **relative pricing framework**, where spreads reveal underlying market structure more clearly than individual price series.

---

## Tools & Technologies

- Python 3  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- yfinance  
- statsmodels (ARIMA, VIF)  
- scikit-learn  

---

## How to Run
pip install pandas numpy matplotlib seaborn yfinance scikit-learn statsmodels
jupyter notebook
energy_market_analysis.ipynb

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/energy-market-analysis.git

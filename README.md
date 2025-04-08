# Analysis
# 🏠 US Housing Trends Analyzer and Influence Explorer

## 📌 Objective
The goal of this project is to model and understand the influence of key national economic factors on U.S. home prices over the past 20 years. Using publicly available data, the project builds predictive models and analyzes feature importance to uncover insights into housing market trends.

---

## 📊 Problem Statement
Home prices in the U.S. are influenced by a wide range of economic, demographic, and policy-related factors. This project seeks to:

- Collect national-level data on these influencing factors.
- Build and evaluate models to predict historical home price trends.
- Analyze which factors have had the most significant impact on housing prices.
- Present findings with clear visualizations.

---

## 🧱 Data Collection

The **S&P Case-Shiller Home Price Index** was used as a proxy for home prices, with data sourced primarily from [FRED (Federal Reserve Economic Data)](https://fred.stlouisfed.org/). The following key economic indicators were collected:

### 🔑 Key Variables:

| Variable | Source |
|---|---|
| **S&P Case-Shiller Home Price Index** | [CSUSHPISA](https://fred.stlouisfed.org/series/CSUSHPISA) |
| **Interest Rates (Federal Funds Rate)** | [FEDFUNDS](https://fred.stlouisfed.org/series/FEDFUNDS) |
| **Unemployment Rate** | [UNRATE](https://fred.stlouisfed.org/series/UNRATE) |
| **Employment Rate** | [LREM64TTUSM156S](https://fred.stlouisfed.org/series/LREM64TTUSM156S) |
| **Working Population** | [LFWA64TTUSM647S](https://fred.stlouisfed.org/series/LFWA64TTUSM647S) |
| **Consumer Price Index (CPI)** | [CPIAUCSL](https://fred.stlouisfed.org/series/CPIAUCSL) |
| **Per Capita GDP** | [A939RX0Q048SBEA](https://fred.stlouisfed.org/series/A939RX0Q048SBEA) |
| **Real Median Household Income** | [MEHOINUSA672N](https://fred.stlouisfed.org/series/MEHOINUSA672N) |
| **Construction Price Index** | [WPUSI012011](https://fred.stlouisfed.org/series/WPUSI012011) |
| **Urban Population Percentage** | [World Bank](https://data.worldbank.org/indicator/SP.URB.TOTL.IN.ZS?end=2021&locations=US&start=2001) |
| **Housing Subsidies (Federal)** | [L312051A027NBEA](https://fred.stlouisfed.org/series/L312051A027NBEA) |
| **Total Number of Households** | [TTLHH](https://fred.stlouisfed.org/series/TTLHH) |

---

## 🛠️ Data Processing

- Cleaned data by handling missing values and standardizing formats.
- Interpolated annual, quarterly, and monthly data to a common frequency.
- Normalized indicators for compatibility across different scales.
- Aligned timelines to a 20-year window (2003–2023) for consistency.

---

## 📈 Exploratory Data Analysis (EDA)

- Plotted time-series trends for all features and target variable.
- Identified correlations between economic indicators and housing prices.
- Visualized lag effects and potential non-linear relationships.

---

## 🤖 Model Development

### ✅ Models Explored:

- **Linear Regression**
- **ElasticNet**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **Support Vector Regression (SVR)**
- **XGBoost Regressor**

Each model was:
- Trained on 80% of the dataset
- Evaluated using **Mean Squared Error (MSE)** and **R-squared (R²)** metrics

---

## 🔍 Feature Importance

For tree-based models like **Random Forest**, **XGBoost**, and **Gradient Boosting**, feature importance was calculated and visualized to determine the most influential predictors.

---

## 📊 Model Comparison

| Model | MSE | R² |
|-------|-----|----|
| Linear Regression | _To be filled_ | _To be filled_ |
| ElasticNet | _To be filled_ | _To be filled_ |
| Random Forest | _To be filled_ | _To be filled_ |
| Gradient Boosting | _To be filled_ | _To be filled_ |
| SVR | _To be filled_ | _To be filled_ |
| XGBoost | _To be filled_ | _To be filled_ |

> **Best Model:** Based on lowest MSE and highest R², the best-performing model was identified to provide accurate predictions and meaningful insights.

---

## 📊 Visualizations

- Time-series plots of actual vs. predicted home prices
- Correlation heatmaps
- Bar plots of feature importances
- Trend plots showing how major indicators changed over time

---

## 📌 Conclusions

- Identified key drivers of home price fluctuations over the last two decades.
- Constructed a reliable model to forecast future price trends based on macroeconomic indicators.
- The project demonstrates the power of public data in understanding national economic dynamics and their impact on real estate.

---

## 📚 References

- 📄 [Investopedia Article on Case-Shiller Index](https://www.investopedia.com/articles/mortgages-real-estate/10/understanding-case-shiller-index.asp)
- 📄 [Research Paper: Factors Influencing Real Estate Prices](https://www.atlantis-press.com/article/25841966.pdf)

---

## 📂 Data Availability

All data used in this project is sourced from publicly available government and international databases, primarily:

- [FRED - Federal Reserve Economic Data](https://fred.stlouisfed.org/)
- [World Bank Open Data](https://data.worldbank.org/)

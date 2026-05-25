# Melbourne House Price Prediction

## Overview
This project applies business analytics and supervised machine learning to predict residential property prices in the Melbourne housing market.

The project follows the CRISP-DM methodology and uses Python, Scikit-learn, Ridge Regression, XGBoost, feature engineering, PCA, correlation analysis, and business-focused visualisation to generate predictive outputs and stakeholder-ready insights.

## Business Problem
Property valuation can be slow, subjective, and inconsistent when based only on manual judgement. A data-driven model can support more reliable initial price estimation by identifying the property and location features most strongly associated with sale price.

This project asks:

**Can machine learning predict Melbourne residential property sale prices using property attributes and location data?**

## Dataset
The project used the Melbourne Housing Market dataset.

Key details:
- 13,580 property records
- 21 raw features
- 641 encoded features after preprocessing
- Target variable: Price in AUD
- Median sale price: approximately AUD 903,000
- Mean sale price: approximately AUD 1,075,684
- Geographic coverage: Greater Melbourne, Australia
- Time period: 2016–2018

## Tools Used
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn
- Power BI
- CRISP-DM

## Methodology
1. Defined the business problem and modelling objective using the CRISP-DM framework.
2. Conducted exploratory data analysis on price distributions, property attributes, location features, and market trends.
3. Treated missing values and logically invalid zero values.
4. Applied one-hot encoding to categorical variables, expanding the dataset to 641 encoded features.
5. Used PCA and correlation analysis to understand feature relationships and dimensionality.
6. Trained Ridge Regression as an interpretable regularised linear baseline.
7. Trained XGBoost Regressor as a non-linear ensemble model to capture complex pricing relationships.
8. Evaluated model performance using MAE, RMSE, R², and MAPE.
9. Interpreted feature importance, residual patterns, and prediction errors for business stakeholders.

## Model Comparison
This project compared a regularised linear model against a non-linear ensemble model:

| Model | MAE (AUD) | RMSE (AUD) | R² Score | MAPE |
|---|---:|---:|---:|---:|
| Ridge Regression | 230,256 | 346,383 | 0.698 | ~21.4% |
| XGBoost Regressor | 162,534 | 270,773 | 0.815 | ~15.1% |
XGBoost substantially outperformed Ridge Regression, showing that Melbourne property prices are better captured through non-linear modelling rather than purely linear assumptions.

## Key Results
- Analysed 13,580 Melbourne property records.
- Engineered 641 encoded features after preprocessing.
- Compared Ridge Regression and XGBoost for residential price prediction.
- XGBoost achieved R² = 0.815, MAE = AUD 162,534, RMSE = AUD 270,773, and MAPE ≈ 15.1%.
- Feature importance analysis showed location and property characteristics as major price drivers.
- Residual and error analysis showed stronger performance on mainstream properties, with larger errors for high-value luxury properties.

## Key Business Insights
- Distance from Melbourne CBD was one of the most important predictors of property price.
- Southern Metropolitan and Eastern Metropolitan regions showed strong price premiums.
- Rooms, bathrooms, bedrooms, building area, and property type were important valuation drivers.
- Detached houses commanded higher average prices than townhouses and units.
- The model performed best for mid-market properties and struggled more with sparse luxury-property cases above AUD 3M.

## Visual Outputs

### Price Distribution
![Price Distribution](images/price_distribution.png)

### Correlation Heatmap
![Correlation Heatmap](images/correlation_heatmap.png)

### Price by Property Type
![Price by Property Type](images/price_by_property_type.png)

### Price by Region
![Price by Region](images/price_by_region.png)

### Price Trends Over Time
![Price Trends Over Time](images/price_trends_over_time.png)

### PCA Price Bands
![PCA Price Bands](images/pca_price_bands.png)

### Predicted vs Actual Prices — Ridge vs XGBoost
![Predicted vs Actual](images/predicted_vs_actual_ridge_xgboost.png)

### Residual Analysis — Ridge vs XGBoost
![Residual Plots](images/residual_plots_ridge_xgboost.png)

### Error Distribution — Ridge vs XGBoost
![Error Distribution](images/error_distribution_ridge_xgboost.png)

### XGBoost Feature Importance
![XGBoost Feature Importance](images/feature_importance_xgboost.png)

### Executive KPI Dashboard
![Executive KPI Dashboard](images/executive_kpi_dashboard.png)

### Key Business Insights Dashboard
![Key Business Insights Dashboard](images/key_business_insights_dashboard.png)

## Business Impact
This project demonstrates how analytics can support:
- More consistent property valuation
- Faster pricing guidance for estate agents
- Investor screening
- Identification of key price drivers
- Clearer communication of pricing evidence to non-technical stakeholders
- More data-backed discussions around property pricing strategy

## Repository Structure
```text
melbourne-house-price-prediction/
├── notebooks/
│   └── melbourne_house_price_prediction.ipynb
├── images/
│   ├── price_distribution.png
│   ├── correlation_heatmap.png
│   ├── price_by_property_type.png
│   ├── price_by_region.png
│   ├── price_trends_over_time.png
│   ├── pca_price_bands.png
│   ├── predicted_vs_actual_ridge_xgboost.png
│   ├── residual_plots_ridge_xgboost.png
│   ├── error_distribution_ridge_xgboost.png
│   ├── feature_importance_xgboost.png
│   ├── executive_kpi_dashboard.png
│   └── key_business_insights_dashboard.png
├── reports/
│   └── business_insights_summary.md
├── data_sample/
│   └── README.md
├── requirements.txt
└── README.md

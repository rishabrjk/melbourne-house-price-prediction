# Melbourne House Price Prediction

## Overview
This project applies business analytics and supervised machine learning to predict residential property prices in the Melbourne housing market.

The project follows the CRISP-DM methodology and uses Python, Scikit-learn, Random Forest, Gradient Boosting, feature engineering, PCA, correlation analysis, and Power BI visualisation to generate both predictive outputs and business insights.

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

## Tools Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Power BI
- CRISP-DM

## Methodology
1. Defined the business problem and modelling objective.
2. Conducted exploratory data analysis on price distributions, property attributes, and location features.
3. Treated missing values and logically invalid zero values.
4. Applied one-hot encoding to categorical variables.
5. Used PCA and correlation analysis to understand feature relationships.
6. Trained Random Forest and Gradient Boosting regression models.
7. Evaluated models using MAE, RMSE, R², and MAPE.
8. Interpreted feature importance and residual patterns for business stakeholders.

## Key Results
- Analysed 13,580 Melbourne property records.
- Engineered 641 encoded features after preprocessing.
- Built supervised regression models for residential price estimation.
- Final model achieved R² of 0.82.
- Built Power BI visuals to communicate feature importance and residual patterns.

## Visual Outputs

### Price Distribution
![Price Distribution](images/price_distribution.png)

### Correlation Heatmap
![Correlation Heatmap](images/correlation_heatmap.png)

### Feature Importance
![Feature Importance](images/feature_importance.png)

### Residual Analysis
![Residual Analysis](images/residual_analysis.png)

### Power BI Dashboard
![Power BI Dashboard](images/powerbi_dashboard.png)

## Business Impact
This project demonstrates how analytics can support:
- More consistent property valuation
- Faster pricing guidance for estate agents
- Investor screening
- Identification of key price drivers
- Clearer communication of pricing evidence to non-technical stakeholders

## Repository Structure
```text
melbourne-house-price-prediction/
├── notebooks/
├── images/
├── reports/
├── data_sample/
├── requirements.txt
└── README.md

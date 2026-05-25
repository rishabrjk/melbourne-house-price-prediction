# Business Insights Summary

## Project Aim
This project explored whether machine learning could support more consistent residential property price estimation in the Melbourne housing market.

## Dataset Overview
- 13,580 property records
- 21 raw features
- 641 encoded features after preprocessing
- Target variable: Price in AUD
- Median sale price: approximately AUD 903,000

## Key Insights
- Number of rooms, bedrooms, bathrooms, and property type were among the strongest indicators of sale price.
- Distance from Melbourne CBD showed a negative relationship with property price, supporting the importance of location.
- Property type and region were important business-facing features for explaining valuation differences.
- PCA showed that the first two components explained 46.8% of total variance, suggesting that simple linear separation was insufficient.

## Model Results
Random Forest and Gradient Boosting models were compared using MAE, RMSE, R², and MAPE.

The final model achieved:
- R²: 0.82

## Business Value
The model could support:
- Initial property valuation estimates
- Estate agent pricing guidance
- Investor screening
- Market comparison analysis
- Data-backed pricing discussions

## Limitations
- The model is based on historical sales data and should not replace professional valuation.
- External macroeconomic variables such as interest rates and inflation were not included.
- Predictions may be weaker for unusual luxury properties or underrepresented suburbs.

# Utility-Company-Regression-Model
# Regression Analysis of Revenue Prediction

## Project Overview
This notebook demonstrates a regression analysis to predict revenue based on production, incorporating seasonal dummy variables for summer and spring.

## Data
The analysis uses the `AICPA_regressionAnalysisData.csv` dataset, which contains `revenue`, `production` data, and a `date` column, along with a `type` column to distinguish between training and testing sets.

## Models
Two separate Ordinary Least Squares (OLS) regression models were developed:

1.  **Summer Model**: This model uses `production` and a `summer_DV` (dummy variable for June, July, August) and `summer_Interaction` (production * summer_DV) to predict revenue. It assesses the impact of the summer season on revenue predictions.

2.  **Spring Model**: Similar to the summer model, this model uses `production`, a `spring_DV` (dummy variable for March, April, May), and `spring_Interaction` (production * spring_DV) to predict revenue, focusing on the spring season's influence.

## Model Assessment
The models were evaluated using the Mean Absolute Percentage Error (MAPE) on a dedicated testing dataset.

*   **Summer Model MAPE**: 19.68%
*   **Spring Model MAPE**: 28.93%

### Visualization
Visualizations are included for both models, illustrating the regression lines for seasonal and non-seasonal periods against actual production and revenue data points.

## Conclusion and Recommendation
The **Summer Model** significantly outperformed the Spring Model, achieving a lower MAPE score of 19.68% compared to the Spring Model's 28.93%. This indicates that the summer dummy variable and its interaction with production provide a more accurate prediction of revenue.

Therefore, the **Summer Model is recommended** for predicting revenue based on the available data and seasonal factors.

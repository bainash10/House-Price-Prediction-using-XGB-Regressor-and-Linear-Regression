# House Price Prediction Using XGB Regressor & Linear Regression

This machine learning project focuses on predicting house prices using a dataset containing various property-related and demographic features. The goal is to build regression models that can accurately estimate housing prices based on factors like location, population, income, and proximity to the ocean. Two models — **XGBoost** and **Linear Regression** — were used and compared to identify the more effective solution.

---

## Project Objective  
To implement and evaluate regression models capable of accurately predicting house prices using real-world housing data from California.

---

## Features Used  

The dataset includes the following features:

- `longitude`  
- `latitude`  
- `housing_median_age`  
- `total_rooms`  
- `total_bedrooms`  
- `population`  
- `households`  
- `median_income`  
- `ocean_proximity` *(Categorical Feature)*  
- `median_house_value` *(Target Variable)*

---

## What Was Done  
- Loaded and explored the housing dataset to understand the structure and distribution of the data.
- Cleaned the dataset by removing rows with missing values using `dropna()`.
- Dropped the categorical column `ocean_proximity` for simplicity and compatibility with the regression models.
- Split the dataset into training and testing sets with a `test_size = 0.20` for unbiased evaluation.
- Trained and evaluated two regression models:
  - **Linear Regression**
  - **XGBoost Regressor**

---

## Regression Model Comparison

| Metric      | XGBoost         | Linear Regression  |
|-------------|------------------|---------------------|
| **R² Score** | 0.8242           | 0.6401              |
| **MAE**      | 32,445.78        | 51,372.67           |
| **MSE**      | 2,403,489,962.70 | 4,921,881,237.63    |
| **RMSE**     | 49,025.40        | 49,025.40           |

---

## Summary of Key Insights
- **XGBoost** achieved a higher **R² score**, meaning it explains more of the variance in house prices.
- **XGBoost** also had lower **MAE** and **MSE**, indicating more accurate and stable predictions.
- Although both models share the same **RMSE**, XGBoost clearly outperformed Linear Regression overall.

---

## Conclusion
- **XGBoost** is better at capturing complex, non-linear relationships in the data and performs more effectively on this dataset.
- **Linear Regression** is simpler and more interpretable but less effective in comparison.

---

**Developed by:** *Nischal Baidar*

# Lab 4: Regression Analysis with Regularization Techniques

## Course
2025 Summer - Advanced Big Data and Data Mining (MSCS-634-B01)

## Lab Title
Lab 4: Regression Analysis with Regularization Techniques

## Purpose
This lab explores the application of different regression models on the Diabetes dataset provided by sklearn. The goal is to understand and compare various regression techniques, particularly focusing on regularization approaches to prevent overfitting and enhance model performance.

## Models Implemented
- Simple Linear Regression (using BMI)
- Multiple Linear Regression (using all features)
- Polynomial Regression (degree=2)
- Ridge Regression
- Lasso Regression

## Evaluation Metrics Used
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared (R²)

## Model Performance Summary

| Model                    | MAE   | MSE     | RMSE  | R²   |
|--------------------------|-------|---------|--------|------|
| Simple Linear Regression | 52.26 | 4061.83 | 63.73 | 0.23 |
| Multiple Regression      | 42.79 | 2900.19 | 53.85 | 0.45 |
| Polynomial Regression    | 52.38 | 4085.03 | 63.91 | 0.23 |
| Ridge Regression         | 42.81 | 2892.03 | 53.78 | 0.45 |
| Lasso Regression         | 42.80 | 2884.55 | 53.71 | 0.46 |

## Key Insights
- BMI is a strong individual predictor, but using multiple features improves accuracy.
- Polynomial regression (degree=2) did not improve performance and slightly increased error, indicating potential overfitting.
- Ridge and Lasso Regression both outperformed standard linear models in terms of generalization.
- Lasso achieved the best R² score (0.46), suggesting it may be useful for feature selection.

## Challenges Faced
- Tuning the regularization parameter (`alpha`) required experimentation.
- Polynomial regression quickly led to overfitting when not properly constrained.
- Visualizing differences between model predictions helped identify generalization quality.

## Conclusion
Regularization techniques like Ridge and Lasso are powerful tools to control overfitting and improve model robustness. The diabetes dataset provided a useful case for understanding when to apply simple vs. complex models.

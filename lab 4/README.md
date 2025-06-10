# Lab 4: Regression Analysis with Regularization Techniques

## Purpose
In this lab, I compared several regression models—including Simple Linear, Multiple Linear, Polynomial, Ridge, and Lasso—on the Diabetes dataset. The goal was to see how well each model predicts disease progression and how regularization affects performance.

## Insights

- Multiple Linear Regression performed best, showing the lowest errors and highest R².
- Using only BMI (Simple Linear Regression) gave poor results, confirming that multiple features are needed.
- Polynomial, Ridge, and Lasso did not improve performance over standard multiple regression.
- Regularization (Ridge/Lasso) did not help much, suggesting the base model was not overfitting.

## Challenges

- All models explained less than half the variance (R² < 0.5), indicating the dataset is complex and may need more features or non-linear models for better predictions.
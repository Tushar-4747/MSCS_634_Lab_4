# MSCS_634_Lab_4 - Regression Analysis with Regularization Techniques

## Overview

This lab demonstrates how to apply multiple regression techniques to the **Diabetes Dataset** from `sklearn.datasets`. The goal is to explore how different regression models perform in predicting disease progression based on various physiological features, and how **regularization techniques** like Ridge and Lasso improve model generalization and prevent overfitting.

---

##  Objectives

- Implement:
  - Simple Linear Regression
  - Multiple Linear Regression
  - Polynomial Regression
  - Ridge Regression
  - Lasso Regression
- Evaluate model performance using:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R-squared (R²)
- Visualize predicted vs actual values for each model.
- Analyze how **regularization parameters** affect model behavior.

---

##  Files Included

| File Name                       | Description                                           |
|--------------------------------|-------------------------------------------------------|
| `Lab_4_Regression_Analysis.ipynb` | Jupyter Notebook with all code, visualizations, and analysis |
| `README.md`                    | This file providing an overview and summary          |

---

##  Dataset

- **Name:** Diabetes dataset (from `sklearn.datasets`)
- **Description:** Contains 10 physiological features (e.g., age, BMI, blood pressure) used to predict a quantitative measure of disease progression one year after baseline.
- **Target Variable:** Disease progression score

---

##  Tools and Libraries

- Python 3.x
- Jupyter Notebook
- scikit-learn
- pandas
- numpy
- seaborn
- matplotlib

---

##  Summary of Results

| Model                    | MAE   | RMSE  | R²    |
|-------------------------|-------|-------|-------|
| Simple Linear Regression (BMI) | ~43  | ~55  | ~0.35 |
| Multiple Linear Regression     | ~42  | ~53  | ~0.45 |
| Polynomial Regression (BMI²)  | ~44  | ~56  | ~0.34 |
| Ridge Regression               | ~42  | ~53  | ~0.44 |
| Lasso Regression               | ~44  | ~55  | ~0.41 |

> *Note: Actual values may vary slightly due to random splitting of the data.*

---

##  Key Insights

- **Multiple Linear Regression** performed best overall by leveraging all features.
- **Polynomial Regression** can overfit if degree is too high.
- **Ridge and Lasso Regression** help regularize the model:
  - Ridge penalizes large coefficients to reduce complexity.
  - Lasso can zero out less important features, acting as a feature selector.
- Overfitting was reduced with Ridge/Lasso compared to Polynomial Regression.

---

## ⚠️ Challenges Faced

- Choosing the appropriate degree for polynomial regression without overfitting.
- Tuning the `alpha` parameter for Ridge and Lasso to balance bias-variance tradeoff.
- Interpreting model performance from multiple evaluation metrics.

---

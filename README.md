# Lab — Building and Evaluating a Linear Regression Model

## Overview

In this lab, you will practice the full machine learning workflow using `scikit-learn`.

You will build a regression model that predicts **medical insurance charges** using demographic and health-related information.

This lab gives you practice with:

- Loading and inspecting a dataset
- Identifying features and a target variable
- Building a simple linear regression model
- Building a multiple linear regression model
- Encoding categorical variables with one-hot encoding
- Splitting data into training and test sets
- Evaluating regression models with MAE, RMSE, and R²
- Comparing model performance
- Interpreting training and test scores

---

## Dataset

For this lab, you will use the **Medical Insurance Cost Prediction** dataset.

The dataset includes the following columns:

| Column | Description |
|---|---|
| `age` | Age of the individual |
| `sex` | Sex of the individual |
| `bmi` | Body mass index |
| `children` | Number of children covered by insurance |
| `smoker` | Whether the individual is a smoker |
| `region` | Residential region |
| `charges` | Medical insurance charges |

The target variable is:

```python
charges
```

Your goal is to predict `charges` using the other columns.

---

## Learning Objectives

By the end of this lab, you will be able to:

- Define features `X` and a target variable `y`
- Use `train_test_split()` to split data into training and test sets
- Train a `LinearRegression` model
- Generate predictions with `.predict()`
- Evaluate regression performance with MAE, RMSE, and R²
- Use `pd.get_dummies()` to one-hot encode categorical variables
- Compare simple and multiple regression models
- Explain whether a model appears to be overfitting, underfitting, or generalizing reasonably well

## Submission Checklist

Before submitting, make sure your notebook includes:

- [ ] Dataset loaded successfully
- [ ] Initial data inspection
- [ ] Simple linear regression model
- [ ] Multiple linear regression model with numeric features
- [ ] One-hot encoded categorical variables
- [ ] Final model using numeric and categorical features
- [ ] MAE, RMSE, and R² for each model
- [ ] Bonus train/test score comparison

---

## Key Takeaways

- Regression models predict numeric values.
- Linear regression can use one feature or multiple features.
- Categorical variables must be converted into numeric columns before modeling.
- `pd.get_dummies()` is one way to one-hot encode categorical variables.
- A train/test split helps evaluate performance on unseen data.
- MAE and RMSE measure prediction error.
- R² measures how much variation the model explains.
- Comparing training and test scores can help identify possible overfitting or underfitting.
- A model should always be evaluated with both metrics and plain-English interpretation.

# AIML Module 5 - Project  
# Critical Analysis: Regression Models for COVID-19 Case Prediction

## Overview

This project focuses on analyzing and comparing different regression approaches for predicting COVID-19 confirmed cases.

The objective is to evaluate how different regression algorithms perform on a real-world dataset and understand the impact of model complexity and regularization.

The models implemented include:

- Linear Regression
- Polynomial Regression
- Ridge Regression
- Lasso Regression
- ElasticNet Regression

The goal is to compare model performance using regression evaluation metrics and identify the model that provides the best prediction capability.

---

# Objectives

- Implement multiple regression algorithms for COVID-19 case prediction
- Compare linear and non-linear regression approaches
- Analyze the impact of polynomial feature expansion
- Understand the role of regularization techniques
- Evaluate models using MAE, MSE, RMSE, and R² Score
- Identify the best-performing regression model
- Analyze the trade-off between model complexity and generalization

---

# Key Concepts

## 1. Linear Regression

A supervised learning algorithm that models the relationship between input variables and the target variable using a linear equation.

Characteristics:

- Simple and interpretable model
- Works well for linear relationships
- Sensitive to outliers
- Limited when handling complex patterns

---

## 2. Polynomial Regression

An extension of linear regression that introduces polynomial features to capture non-linear relationships.

Characteristics:

- Handles complex patterns
- Provides better fitting for non-linear trends
- Higher polynomial degrees may cause overfitting
- Requires careful model selection

---

## 3. Ridge Regression

A regularized regression technique that reduces overfitting by adding an L2 penalty term.

Characteristics:

- Improves model stability
- Handles multicollinearity
- Prevents excessive weight growth
- Provides better generalization

---

## 4. Lasso Regression

A regression method using L1 regularization that can reduce unnecessary feature contributions.

Characteristics:

- Performs feature selection
- Produces simpler models
- Helps reduce overfitting
- Useful for high-dimensional data

---

## 5. ElasticNet Regression

A combination of Ridge and Lasso regularization.

Characteristics:

- Balances L1 and L2 penalties
- Provides stable predictions
- Handles correlated features effectively

---

# Dataset

The COVID-19 dataset is used for regression analysis.

Dataset Source:

COVID-19 Data Repository  
https://raw.githubusercontent.com/PranavTadimeti/Regression_Project/main/covid_19_data.csv


## Dataset Characteristics:

- Real-world COVID-19 case records
- Contains confirmed cases, deaths, and recovered cases
- Represents continuously changing real-world trends
- Contains non-linear growth patterns

---

# Experiments Performed

## Experiment 1: Linear Regression Analysis

A baseline Linear Regression model was trained and evaluated.

Evaluation Metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score

Observation:

- Provides a simple baseline prediction
- Struggles with complex growth patterns

---

## Experiment 2: Polynomial Regression Analysis

Polynomial features were introduced to capture non-linear COVID-19 growth trends.

Observation:

- Captures complex relationships better than simple linear regression
- Higher complexity may increase overfitting risk

---

## Experiment 3: Regularized Regression Comparison

Regularization techniques were applied:

- Ridge Regression
- Lasso Regression
- ElasticNet Regression

Observation:

- Regularization improves model stability
- Reduces overfitting
- Provides better generalization on unseen data

---

# Model Evaluation

Models were evaluated using:

## Mean Absolute Error (MAE)

Measures the average magnitude of prediction errors.

Lower MAE indicates better performance.

---

## Mean Squared Error (MSE)

Measures squared difference between actual and predicted values.

Lower MSE indicates fewer large prediction errors.

---

## Root Mean Squared Error (RMSE)

Measures prediction error magnitude while maintaining original units.

Lower RMSE indicates improved prediction accuracy.

---

## R² Score

Measures how well the model explains the variance in the dataset.

Higher R² indicates better model performance.

---

# Results and Insights

The analysis shows:

- Linear Regression provides a strong baseline model
- Polynomial Regression captures non-linear COVID-19 trends effectively
- Ridge Regression improves stability through regularization
- Lasso Regression reduces unnecessary feature impact
- ElasticNet combines the advantages of Ridge and Lasso
- Regularized models generally provide better generalization

The best-performing model is selected based on the highest R² Score and lowest error values.

---

# Model Comparison

The implemented models are compared based on:

| Model | MAE | MSE | R² Score |
|-------|-----|-----|----------|
| Linear Regression | - | - | - |
| Polynomial Regression | - | - | - |
| Ridge Regression | - | - | - |
| Lasso Regression | - | - | - |
| ElasticNet Regression | - | - | - |

---

# Conclusion

This project demonstrates that:

- Different regression algorithms behave differently on real-world datasets
- Polynomial models are useful for capturing non-linear relationships
- Regularization improves model reliability and reduces overfitting
- Evaluation metrics are essential for selecting the best regression model
- Model selection depends on balancing complexity and generalization

Understanding regression techniques helps in building reliable predictive systems for real-world applications.

---

# Author

**Shreya Sari**  
AIML Training Program – Module 5 Project

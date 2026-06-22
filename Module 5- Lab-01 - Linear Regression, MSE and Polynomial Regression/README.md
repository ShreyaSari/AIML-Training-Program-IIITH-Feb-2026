# AIML Module 5 – Lab 01

## Linear Regression, MSE and Polynomial Regression

---

## Overview

This lab introduces fundamental regression techniques used in machine learning for predicting continuous values.

The lab explores:

* Linear Regression
* Mean Squared Error (MSE)
* Polynomial Regression
* Model Evaluation using RMSE and R² Score
* California Housing Dataset Analysis
* Overfitting in High-Degree Polynomial Models

The objective is to understand how regression models learn relationships from data and how model complexity affects performance.

---

## Objectives

* Understand the concept of Linear Regression
* Learn how regression models fit data using best-fit lines
* Analyze prediction error using Mean Squared Error (MSE)
* Compare Linear and Polynomial Regression models
* Apply regression techniques to a real-world housing dataset
* Understand overfitting and underfitting behavior

---

## Key Concepts

### 1. Linear Regression

Linear Regression models the relationship between an input variable and an output variable using a straight line:

**y = mx + c**

Where:

* m = slope (coefficient)
* c = intercept

The model learns values of m and c that minimize prediction error.

Advantages:

* Simple and interpretable
* Fast training
* Effective for linear relationships

---

### 2. Mean Squared Error (MSE)

Mean Squared Error is one of the most common loss functions used in regression.

It measures the average squared difference between actual and predicted values.

Characteristics:

* Penalizes large errors heavily
* Used during model optimization
* Lower MSE indicates better model performance

---

### 3. Polynomial Regression

Polynomial Regression extends Linear Regression by introducing polynomial features.

Example:

**y = a₀ + a₁x + a₂x² + ... + aₙxⁿ**

Advantages:

* Captures non-linear relationships
* Provides better fitting for curved data patterns

Limitations:

* High-degree polynomials may overfit noisy data
* Reduced generalization on unseen data

---

## Datasets Used

### Synthetic Regression Dataset

Generated using:

* Linear relationship with added noise
* Polynomial relationship with added noise

Purpose:

* Visualize regression behavior
* Compare model fitting performance

---

### California Housing Dataset

Real-world housing dataset containing:

* Median Income
* House Age
* Average Rooms
* Average Bedrooms
* Population
* Average Occupancy
* Latitude
* Longitude

Target Variable:

* Median House Value (MEDV)

---

## Experiments Performed

### Experiment 1: Brute Force Line Search

A naive approach was used to search multiple values of:

* Slope (m)
* Intercept (c)

Observation:

* Produces approximate solutions
* Computationally inefficient
* Does not guarantee optimal parameters

---

### Experiment 2: Linear Regression on Noisy Linear Data

A Linear Regression model was trained on synthetic data.

Observation:

* Learned line closely matches actual trend
* Provides accurate predictions
* Efficient compared to brute-force search

---

### Experiment 3: Error Analysis using MSE

Mean Squared Error was used to evaluate prediction quality.

Observation:

* Lower MSE corresponds to better fitting models
* Useful for comparing regression models

---

### Experiment 4: Polynomial Regression

Polynomial Regression was applied to non-linear data.

Observation:

* Linear Regression failed to capture curvature
* Polynomial Regression successfully modeled the pattern
* Significant improvement in prediction accuracy

---

### Experiment 5: California Housing Price Prediction

Linear Regression was trained using the California Housing Dataset.

Steps:

* Data exploration
* Correlation analysis
* Feature selection
* Model training
* Performance evaluation

Observation:

* Median Income showed the strongest positive correlation with house prices
* Linear Regression provided reasonable predictions

---

### Experiment 6: Overfitting Analysis

Higher-degree polynomial models were trained on noisy sine-wave data.

Observation:

* Low-degree models underfit the data
* High-degree models overfit noise and outliers
* Moderate polynomial degrees provide better generalization

---

## Results and Insights

* Linear Regression performs well when relationships are approximately linear.
* Mean Squared Error is an effective metric for measuring prediction quality.
* Polynomial Regression can model complex non-linear patterns.
* Increasing polynomial degree improves flexibility but may cause overfitting.
* Feature correlation analysis helps identify important predictors.
* Median Income is a strong predictor of housing prices in the California Housing Dataset.
* Model complexity should be chosen carefully to balance bias and variance.

---

## Conclusion

This lab demonstrates the foundations of regression modeling and prediction.

Key takeaways:

* Linear Regression is simple, efficient, and interpretable.
* MSE provides a quantitative measure of prediction error.
* Polynomial Regression extends Linear Regression to handle non-linear data.
* Real-world datasets often require careful feature analysis.
* Excessive model complexity can lead to overfitting.

Understanding these concepts is essential for building predictive machine learning systems and forms the basis for more advanced regression and optimization techniques.

---

## Author

Shreya Sari
AIML Training Program – Module 5 Lab 01

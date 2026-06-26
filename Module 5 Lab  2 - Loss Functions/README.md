# AIML Module 5 - Lab 2

# Critical Analysis: Loss Functions and KNN Regression

## Overview

This lab focuses on understanding different loss functions used in regression problems and analyzing their impact on model performance.

The experiments explore:

* Regression loss functions
* Error measurement techniques
* Robust loss functions
* KNN Regression performance
* Effect of different K values on model accuracy

The goal is to understand how different evaluation metrics and hyperparameter choices influence machine learning model behavior.

---

# Objectives

* Understand different regression loss functions
* Compare MSE, MAE, and RMSE performance
* Analyze the effect of different loss functions on prediction errors
* Explore robust loss functions such as Huber Loss
* Implement KNN Regression on real-world datasets
* Identify the optimal value of K for KNN Regression
* Study the effect of extreme K values:

  * K = 1
  * K = size of training dataset

---

# Key Concepts

## 1. Mean Squared Error (MSE)

MSE calculates the average squared difference between actual and predicted values.

Formula:

```
MSE = Σ(y - ŷ)² / n
```

Characteristics:

* Penalizes large errors heavily
* Sensitive to outliers
* Commonly used for regression optimization
* Encourages models to minimize large prediction mistakes

---

## 2. Mean Absolute Error (MAE)

MAE calculates the average absolute difference between actual and predicted values.

Formula:

```
MAE = Σ|y - ŷ| / n
```

Characteristics:

* More robust to outliers
* Treats all errors equally
* Easier to interpret
* Provides stable performance on noisy datasets

---

## 3. Root Mean Squared Error (RMSE)

RMSE is the square root of MSE.

Formula:

```
RMSE = √MSE
```

Characteristics:

* Maintains original target variable units
* Penalizes large errors
* Useful for comparing regression models

---

## 4. Huber Loss

Huber Loss combines the advantages of MSE and MAE.

Characteristics:

* Behaves like MSE for small errors
* Behaves like MAE for large errors
* More resistant to outliers
* Useful for noisy real-world datasets

---

# Dataset

## Regression Dataset

The experiments use regression datasets from Scikit-Learn.

Dataset characteristics:

* Continuous target variable
* Multiple numerical features
* Suitable for regression analysis

---

# Experiments Performed

## Experiment 1: Regression Loss Function Comparison

Different loss functions were evaluated using a regression model.

Metrics compared:

* Mean Squared Error
* Root Mean Squared Error
* Mean Absolute Error

### Observation:

* MSE gives higher penalty to large prediction errors.
* MAE provides more stable results when outliers exist.
* RMSE provides an interpretable measure of prediction error.

---

# Experiment 2: Exploring Additional Loss Function

## Huber Loss Analysis

Huber Loss was implemented and compared with traditional regression losses.

### Observation:

* Huber Loss provides a balance between MSE and MAE.
* It reduces the impact of extreme errors.
* It is useful when datasets contain noisy observations.

---

# Experiment 3: KNN Regression Analysis

K-Nearest Neighbor Regression was implemented and tested with different K values.

Different values of K were evaluated:

```
K = 1 to 30
```

The best K value was selected based on minimum RMSE.

### Observation:

* Small K values capture local patterns.
* Large K values create smoother predictions.
* Optimal K provides the best balance between bias and variance.

---

# Experiment 4: Effect of Extreme K Values

Two extreme cases were tested:

## Case 1: K = 1

Observation:

* Model depends only on the nearest training sample.
* Low bias but high variance.
* Can lead to overfitting.

---

## Case 2: K = Complete Training Dataset Size

Observation:

* Prediction is based on all training samples.
* Produces overly generalized predictions.
* Can lead to underfitting.

---

# Results and Insights

The experiments demonstrate:

* Loss functions strongly influence model evaluation.
* MSE is effective but sensitive to large errors.
* MAE provides better robustness against outliers.
* Huber Loss combines stability and accuracy.
* KNN performance depends heavily on selecting the correct K value.
* Extreme values of K negatively affect generalization.

---

# Model Evaluation

Models were evaluated using:

| Metric | Purpose                                     |
| ------ | ------------------------------------------- |
| MAE    | Measures average absolute prediction error  |
| MSE    | Penalizes large errors                      |
| RMSE   | Measures prediction error in original units |

---

# Conclusion

This lab demonstrates that:

* Selecting appropriate loss functions is important for regression performance.
* Different loss functions influence model behavior differently.
* Robust losses improve performance on noisy datasets.
* KNN Regression requires careful selection of K.
* Very small K values cause overfitting.
* Very large K values cause underfitting.

Understanding loss functions and hyperparameter selection helps build reliable machine learning models for real-world regression problems.

---

# Author

**Shreya Sari**
AIML Training Program – Module 5 Lab 2

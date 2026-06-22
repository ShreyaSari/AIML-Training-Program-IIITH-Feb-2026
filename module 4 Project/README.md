# AIML Module 4 - Project
## Critical Analysis: Perceptron, Margin Models & Gradient Descent

---

## Overview

This lab focuses on comparing different classification and optimization approaches including:

- Perceptron Learning Algorithm
- Margin-based classification model
- Gradient Descent optimization model

The goal is to analyze their convergence behavior, accuracy performance, and robustness on a noisy dataset such as the Water Potability dataset.

---

## Objectives

- Compare convergence behavior of Perceptron and Gradient Descent
- Analyze cost reduction over training iterations
- Evaluate model accuracy on test data
- Understand the impact of learning rate
- Study robustness of margin-based classifiers
- Interpret behavior on noisy datasets

---

## Key Concepts

### 1. Perceptron Algorithm
A linear classifier that updates weights only when misclassification occurs.

- Simple and fast
- Sensitive to noisy data
- Does not optimize margin

---

### 2. Gradient Descent Optimization
An iterative optimization method that minimizes a loss function.

- Uses continuous gradient updates
- Smooth convergence curve
- Sensitive to learning rate

---

### 3. Margin-Based Classification
A classifier that maximizes the distance between decision boundary and data points.

- Strong generalization
- Robust to noise and outliers
- Preferred for real-world datasets

---

## Dataset

The **Water Potability Dataset** is used for evaluation.

Characteristics:
- Contains noisy and overlapping classes
- Binary classification problem
- Real-world imbalanced patterns

---

## Experiments Performed

### Experiment 1: Convergence Analysis
- Perceptron mistake history plotted
- Gradient Descent cost history plotted

Observation:
- Perceptron → irregular convergence
- Gradient Descent → smooth convergence

---

### Experiment 2: Accuracy Comparison
Test accuracy evaluated for all models:

- Perceptron Model
- Margin-based Model
- Gradient Descent Model

Observation:
- Margin-based model performs best in noisy environments

---

### Experiment 3: Noise Robustness
Models tested on Water Potability dataset.

Observation:
- Perceptron struggles with noisy boundary points
- Margin-based model remains stable and robust

---

## Results and Insights

- Gradient Descent provides smooth optimization curves
- Perceptron is sensitive to sample ordering and noise
- Margin-based models generalize better on real-world data
- High learning rate causes instability in optimization
- Label encoding {-1, +1} simplifies mathematical formulation

---

## Conclusion

This lab demonstrates that:

- Optimization methods significantly impact model performance
- Margin-based classifiers are most robust for noisy datasets
- Gradient Descent provides stable convergence behavior
- Proper learning rate selection is critical for success

Understanding these differences helps in selecting the right model for real-world machine learning problems.

---

## Author

Shreya Sari  
AIML Training Program – Module 4 Project

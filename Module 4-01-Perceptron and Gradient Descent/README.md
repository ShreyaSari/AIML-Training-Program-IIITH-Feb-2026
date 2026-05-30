# AIML Module 4 – Lab 01

## Perceptron and Gradient Descent

## Overview

This lab introduces the **Perceptron Learning Algorithm**, one of the earliest supervised machine learning algorithms used for binary classification. The notebook demonstrates how a Perceptron learns a linear decision boundary by iteratively updating weights based on classification errors.

The lab also explores the concept of **Gradient Descent**, a fundamental optimization technique used to minimize error functions and train machine learning models efficiently.

Through visualization and experimentation, students gain practical understanding of linear separability, weight updates, decision boundaries, convergence behavior, and optimization methods.

---

## Objectives

The primary objectives of this lab are:

* Understand the fundamentals of the Perceptron algorithm
* Learn how binary classification works
* Understand linear separability in datasets
* Implement the Perceptron learning rule
* Visualize decision boundaries
* Track training error during learning
* Understand convergence of the Perceptron algorithm
* Learn the basics of Gradient Descent optimization
* Analyze how model parameters are updated iteratively

---

## Dataset

A small toy dataset is used for demonstration purposes.

The dataset contains:

* Two input features (x₁ and x₂)
* Binary class labels (+1 and -1)
* Linearly separable samples

The dataset is used to:

* Train a Perceptron classifier
* Visualize classification boundaries
* Observe weight updates during training
* Analyze model convergence

---

## Key Concepts Covered

### 1. Perceptron

The Perceptron is one of the simplest supervised learning algorithms for binary classification.

It attempts to find a linear boundary that separates two classes.

The Perceptron computes:

```text
Output = sign(w · x + b)
```

Where:

* **w** = Weight vector
* **x** = Input features
* **b** = Bias term

The output belongs to either:

* +1 (Positive Class)
* -1 (Negative Class)

---

### 2. Linear Separability

A dataset is said to be linearly separable if a straight line (or hyperplane in higher dimensions) can separate samples from different classes.

Characteristics:

* Positive and negative samples are separable by a single decision boundary.
* Perceptron converges only when the dataset is linearly separable.

Examples:

* AND function → Linearly separable
* OR function → Linearly separable
* XOR function → Not linearly separable

---

### 3. Perceptron Learning Rule

The Perceptron learns by updating its weights whenever it misclassifies a sample.

Weight update equation:

```text
w(new) = w(old) + ηyx
```

Bias update equation:

```text
b(new) = b(old) + ηy
```

Where:

* **η** = Learning rate
* **y** = Actual label
* **x** = Input vector

The objective is to reduce classification errors and correctly separate the classes.

---

### 4. Training Process

The Perceptron training process follows these steps:

1. Initialize weights to zero.
2. Pass each sample through the model.
3. Predict its class.
4. Compare prediction with actual label.
5. Update weights if misclassified.
6. Repeat until convergence or maximum epochs are reached.

This iterative learning process gradually improves classification performance.

---

### 5. Error Tracking

Training error is monitored across multiple epochs.

Benefits of error tracking:

* Helps visualize learning progress.
* Confirms convergence.
* Shows whether the algorithm is improving over time.

A decreasing error curve indicates successful learning.

---

### 6. Decision Boundary Visualization

The trained weight vector defines a decision boundary.

The notebook visualizes:

* Positive samples
* Negative samples
* Learned separating line
* Test samples

This provides an intuitive understanding of how the Perceptron classifies data.

---

### 7. Gradient Descent

Gradient Descent is an optimization algorithm used to minimize a loss function.

The basic update rule is:

```text
θ = θ − α ∇J(θ)
```

Where:

* **θ** = Model parameters
* **α** = Learning rate
* **∇J(θ)** = Gradient of the loss function

Gradient Descent repeatedly moves parameters in the direction that reduces prediction error.

---

### 8. Convergence

The Perceptron Convergence Theorem states:

* If the dataset is linearly separable, the Perceptron will converge after a finite number of updates.
* If the dataset is not linearly separable, convergence is not guaranteed.

This concept explains why some classification problems are easy to solve while others require more advanced neural networks.

---

## Results and Insights

Key observations from the experiments:

* The Perceptron successfully learns linearly separable datasets.
* Weight updates occur only when misclassifications are made.
* Training error decreases as learning progresses.
* Decision boundaries become more accurate after multiple epochs.
* Gradient Descent provides a systematic way to minimize errors.
* Non-linearly separable datasets cannot be solved using a single-layer Perceptron.

---

## Applications

Perceptrons and Gradient Descent form the foundation of many machine learning systems, including:

* Neural Networks
* Deep Learning Models
* Image Classification
* Speech Recognition
* Natural Language Processing
* Recommendation Systems
* Fraud Detection
* Medical Diagnosis Systems

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* Google Colab

---

## Project Workflow

```text
Dataset
   ↓
Initialize Weights
   ↓
Forward Prediction
   ↓
Check Classification Error
   ↓
Update Weights
   ↓
Repeat for Multiple Epochs
   ↓
Convergence
   ↓
Visualize Decision Boundary
```

---

## Conclusion

This lab provides a practical introduction to the Perceptron Learning Algorithm and Gradient Descent. By training a Perceptron on a linearly separable dataset, we observe how weights are updated iteratively to reduce classification errors and create an effective decision boundary.

The experiments highlight the importance of linear separability, convergence, and optimization in machine learning. Understanding these concepts forms the foundation for studying more advanced neural networks and deep learning architectures.

---

## Author

**Shreya Sari**
*AIML Training Program – Module 4 Lab 01*

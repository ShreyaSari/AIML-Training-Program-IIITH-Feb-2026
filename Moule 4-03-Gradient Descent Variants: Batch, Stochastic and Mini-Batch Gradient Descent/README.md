# AIML Module 4 – Lab 03

# Gradient Descent Variants: Batch, Stochastic and Mini-Batch Gradient Descent

## Overview

This lab explores different variants of Gradient Descent optimization algorithms used in Machine Learning for minimizing loss functions and optimizing model parameters.

The notebook demonstrates how optimization algorithms update model parameters iteratively to reduce prediction error in regression problems. It focuses on understanding the differences between **Batch Gradient Descent, Stochastic Gradient Descent (SGD), and Mini-Batch Gradient Descent**.

The lab also analyzes the effect of batch size, learning rate selection, learning rate scheduling, and convergence behavior on model performance.

Through practical implementation and experimentation, students understand how different optimization strategies impact training speed, stability, and accuracy.

---

# Objectives

The primary objectives of this lab are:

- Understand different variants of Gradient Descent optimization
- Implement Batch Gradient Descent from scratch
- Implement Stochastic Gradient Descent (SGD)
- Implement Mini-Batch Gradient Descent
- Compare convergence behavior of different optimization methods
- Analyze the effect of batch size on training performance
- Study the impact of learning rates on optimization
- Implement learning rate scheduling techniques
- Understand the role of data shuffling in Mini-Batch Gradient Descent
- Analyze optimization behavior for convex loss functions

---

# Dataset

A synthetic regression dataset is used to demonstrate optimization techniques.

The dataset contains:

- Input feature values
- Continuous target values
- Regression relationships with added noise

The dataset is used to:

- Train regression models
- Calculate prediction errors
- Compute gradients
- Update model parameters
- Compare optimization algorithms
- Visualize convergence behavior

---

# Key Concepts Covered

## 1. Gradient Descent Variants

Gradient Descent is an optimization algorithm that minimizes a loss function by updating model parameters in the opposite direction of the gradient.

The parameter update rule is:

\[
\theta = \theta - \alpha \nabla J(\theta)
\]

Where:

- θ = Model parameters
- α = Learning rate
- ∇J(θ) = Gradient of the loss function

Different variants modify how training samples are used to calculate gradients.

---

# 2. Batch Gradient Descent

Batch Gradient Descent calculates gradients using the complete training dataset before updating parameters.

### Characteristics:

- Uses all samples for every update
- Provides accurate gradient estimation
- Produces smooth convergence
- Requires more computational resources for large datasets

### Advantages:

- Stable optimization
- Deterministic updates
- Suitable for small datasets

### Limitations:

- Slow for very large datasets
- High memory requirements

---

# 3. Stochastic Gradient Descent (SGD)

Stochastic Gradient Descent updates parameters using only one randomly selected training sample at a time.

### Characteristics:

- Frequent parameter updates
- Faster learning in early stages
- Noisy convergence behavior

### Advantages:

- Faster computation
- Works well with large datasets
- Can escape local minima due to randomness

### Limitations:

- High variance updates
- Requires careful learning rate tuning

---

# 4. Mini-Batch Gradient Descent

Mini-Batch Gradient Descent combines the advantages of Batch GD and SGD.

Instead of using the complete dataset or a single sample, it uses small batches of training examples.

### Characteristics:

- Faster than Batch GD
- More stable than SGD
- Efficient memory usage
- Commonly used in deep learning

### Effect of Batch Size:

Small batch size:

- Faster updates
- More noise in loss curve
- Less stable convergence

Large batch size:

- Smoother optimization
- More stable convergence
- Higher computational cost

When batch size equals the total number of samples, Mini-Batch Gradient Descent becomes equivalent to Batch Gradient Descent.

---

# 5. Learning Rate Analysis

The learning rate controls the size of parameter updates.

### Small Learning Rate:

- Slow convergence
- Requires more iterations

### Large Learning Rate:

- Overshooting of minimum
- Possible divergence
- Unstable loss curve

### Optimal Learning Rate:

- Faster convergence
- Stable optimization
- Lower final error

SGD is generally more sensitive to learning rate changes because updates are based on individual samples.

---

# 6. Learning Rate Scheduling

Learning rate scheduling gradually decreases the learning rate during training.

Example:

\[
lr = \frac{initial\_lr}{epoch+1}
\]

Benefits:

- Reduces oscillations
- Improves convergence stability
- Helps SGD approach the minimum more accurately

---

# 7. Data Shuffling

Data shuffling is important in Mini-Batch Gradient Descent.

Benefits:

- Prevents biased batches
- Creates better gradient estimates
- Improves generalization
- Provides representative training batches

Randomizing data order before every epoch improves optimization performance.

---

# 8. Convex and Non-Convex Optimization

## Convex Loss Functions

A convex loss function contains a single global minimum.

Characteristics:

- Easy optimization
- No local minima problems
- Gradient-based methods converge effectively

Example:

Linear Regression using Mean Squared Error.

---

## Non-Convex Loss Functions

Non-convex functions may contain:

- Multiple local minima
- Saddle points
- Flat regions

Deep Neural Networks commonly have non-convex optimization landscapes.

Optimization becomes more challenging because finding the global minimum is difficult.

---

# 9. Convergence Analysis

Convergence occurs when:

- Loss value stops decreasing
- Parameter updates become very small
- Model reaches minimum error

Factors affecting convergence:

- Learning rate
- Batch size
- Dataset size
- Optimization algorithm
- Initial parameters

---

# Implementation Workflow
<img width="358" height="603" alt="image" src="https://github.com/user-attachments/assets/952b8956-bf68-4e1e-8a3e-02a747e7e25a" />


---

# Experiments Performed

## Experiment 1: Batch Size Comparison

Different mini-batch sizes are tested.

Observations:

- Small batch sizes create noisy loss curves.
- Large batch sizes produce smoother convergence.
- Full dataset batch size behaves like Batch Gradient Descent.

---

## Experiment 2: Learning Rate Comparison

Different learning rates are evaluated.

Observations:

- Very low learning rates converge slowly.
- Very high learning rates may prevent convergence.
- Proper learning rate improves optimization efficiency.

---

## Experiment 3: Learning Rate Scheduling

A decreasing learning rate is applied to SGD.

Observations:

- Training becomes more stable.
- Oscillations reduce.
- Final error improves.

---

# Results and Insights

Key observations from experiments:

- Batch Gradient Descent provides stable convergence.
- SGD provides faster updates but introduces noise.
- Mini-Batch Gradient Descent provides a balance between speed and stability.
- Batch size significantly affects convergence behavior.
- Learning rate selection is critical for successful optimization.
- Learning rate scheduling improves SGD performance.
- Data shuffling improves mini-batch quality.
- Convex optimization problems have a unique global optimum.

---

# Applications

Gradient Descent variants are widely used in:

- Linear Regression
- Logistic Regression
- Neural Networks
- Deep Learning
- Computer Vision
- Natural Language Processing
- Recommendation Systems
- Fraud Detection
- Healthcare Analytics
- Predictive Modeling

---

# Technologies Used

- Python
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- Google Colab

---

# Conclusion

This lab provides a practical understanding of different Gradient Descent optimization techniques and their impact on Machine Learning model training.

Through implementation of Batch Gradient Descent, Stochastic Gradient Descent, and Mini-Batch Gradient Descent, students learn how optimization algorithms update parameters and minimize loss functions.

The experiments demonstrate the importance of learning rate selection, batch size, data shuffling, and convergence analysis.

Understanding these optimization methods provides the foundation required for training advanced Machine Learning and Deep Learning models.

---

# Author

**Shreya Sari**  
**AIML Training Program – Module 4 Lab 03**

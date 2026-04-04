# AIML Module 1 – Lab 04

## Transforming Data using Linear Algebra

---

## Overview

This notebook explores the application of **linear algebra techniques** in transforming data for machine learning tasks. The goal of this lab is to understand how feature transformations influence model performance and help improve classification results.

The notebook demonstrates how different mathematical transformations can reshape feature spaces and affect the behavior of a **Nearest Neighbor (NN)** classifier.

---

## Objectives

The main objectives of this lab are:

* Understand the role of **linear transformations** in machine learning
* Learn how feature space transformations impact model performance
* Implement and analyze different transformation matrices
* Explore the effect of **feature scaling and normalization**
* Evaluate model performance using transformed and original features

---

## Dataset

The dataset used in this notebook consists of image data processed within the notebook. From each image, key features are extracted:

* **Hole Pixels** → represents internal structure of the image
* **Boundary Pixels** → represents the outer structure of the image

These features form a 2D feature space used for classification.

---

## Key Concepts Covered

### 1. Linear Transformations

Linear transformations involve applying matrix operations to feature vectors to modify their representation in space.

The notebook applies:

* Identity Transformation
* Scaling Transformation
* Shear/Rotation Transformation

These transformations help analyze how data distribution changes in feature space.

---

### 2. Feature Representation

The model uses:

* Hole pixels
* Boundary pixels

These features are combined to form input vectors for classification.

---

### 3. Normalization

Normalization standardizes feature values to ensure they are on the same scale. This prevents bias toward features with larger magnitudes and improves model stability.

---

### 4. Model Evaluation

A **Nearest Neighbor (NN)** classifier is used to evaluate performance. The notebook compares results across:

* Original feature space
* Transformed feature space
* Normalized feature space

---

## Results and Insights

Key observations from the experiments:

* Linear transformations significantly affect model accuracy
* Certain transformations improve class separability
* Poor transformations can distort data and reduce performance
* Normalization improves consistency and stability
* Feature representation plays a critical role in classification

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* TensorFlow / Keras
* Jupyter Notebook / Google Colab

---

## Conclusion

This lab provides a practical understanding of how **linear algebra concepts** are applied in machine learning. By transforming and analyzing feature spaces, we observe how mathematical operations directly impact model performance and decision boundaries.

---

## Author

**Shreya Sari**
AIML Training Program – Module 1 Lab 04

---

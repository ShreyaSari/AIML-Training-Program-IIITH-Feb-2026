# AIML Module 3 – Lab 01

## Understanding Distance Metrics and Introduction to KNN

---

## Overview

This notebook introduces the fundamental concepts of **distance metrics** and their importance in machine learning algorithms, particularly the **K-Nearest Neighbors (KNN)** algorithm.

The lab focuses on understanding how similarity and distance measurements influence classification tasks and how different distance metrics affect the behavior of machine learning models.

---

## Objectives

The main objectives of this lab are:

* Understand the concept of distance and similarity
* Learn the mathematical properties of distance metrics
* Explore common distance measures used in machine learning
* Understand the working of the K-Nearest Neighbors (KNN) algorithm
* Analyze how distance metrics affect classification performance
* Compare similarity and distance-based approaches

---

## Dataset

The notebook uses sample datasets for classification and visualization tasks.

The datasets are analyzed using different distance metrics to understand neighborhood relationships between data points.

---

## Key Concepts Covered

### 1. Distance Metrics

Distance metrics measure how far apart two data points are.

Common distance metrics explored include:

* Euclidean Distance
* Manhattan Distance
* Minkowski Distance

These metrics are widely used in machine learning for clustering and classification.

---

### 2. Similarity Measures

Similarity measures determine how alike two data points are.

Examples include:

* Cosine Similarity
* Jaccard Similarity

Higher similarity values indicate stronger relationships between data points.

---

### 3. Difference Between Similarity and Distance

#### Similarity
* Measures likeness between objects
* Higher value means more similar

#### Distance
* Measures dissimilarity between objects
* Lower value means more similar

Both concepts are essential in machine learning and data analysis.

---

### 4. Properties of Distance Metrics

For a function to be considered a valid distance metric, it must satisfy:

* Non-Negativity
* Identity of Indiscernibles
* Symmetry
* Triangle Inequality

These properties ensure reliable distance calculations.

---

### 5. K-Nearest Neighbors (KNN)

KNN is a supervised machine learning algorithm used for classification and regression.

The algorithm works by:

* Finding the nearest neighbors
* Measuring distances between data points
* Predicting labels based on nearby samples

---

## Results and Insights

Key observations from the experiments:

* Distance metrics significantly influence KNN performance
* Feature scaling affects distance calculations
* Different metrics behave differently depending on data distribution
* Similarity and distance are inversely related concepts
* Proper metric selection improves classification accuracy

---

## Applications

Distance metrics and KNN are widely used in:

* Recommendation Systems
* Image Recognition
* Pattern Recognition
* Customer Segmentation
* Medical Diagnosis
* Anomaly Detection

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* Scikit-learn
* Pandas
* Jupyter Notebook / Google Colab

---

## Conclusion

This lab provides a foundational understanding of distance metrics and similarity measures in machine learning. By exploring KNN and various distance functions, we observe how mathematical distance calculations directly influence classification and neighborhood-based learning algorithms.

Understanding these concepts is essential for building effective machine learning models and selecting appropriate similarity measures for different datasets.

---

## Author

**Shreya Sari**  
AIML Training Program – Module 3 Lab 01

---

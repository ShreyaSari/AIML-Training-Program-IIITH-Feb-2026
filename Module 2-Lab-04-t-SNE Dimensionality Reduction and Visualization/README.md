# AIML Module 2 – Lab 04

## t-SNE Dimensionality Reduction and Visualization

---

## Overview

This notebook explores the **t-Distributed Stochastic Neighbor Embedding (t-SNE)** algorithm for non-linear dimensionality reduction and data visualization. The objective of this lab is to understand how t-SNE transforms high-dimensional datasets into lower-dimensional representations while preserving meaningful neighborhood relationships.

The notebook compares t-SNE with PCA and demonstrates how non-linear dimensionality reduction techniques reveal hidden patterns and clusters in complex datasets.

---

## Objectives

The main objectives of this lab are:

* Understand the concept of dimensionality reduction
* Learn the working principles of t-SNE
* Compare PCA and t-SNE
* Analyze local and global structure preservation
* Study the impact of hyperparameters on visualization
* Visualize high-dimensional datasets effectively

---

## Dataset

The notebook uses high-dimensional datasets for visualization and manifold analysis.

The datasets are projected into lower-dimensional spaces using:

* PCA
* t-SNE

to compare visualization quality and clustering behavior.

---

## Key Concepts Covered

### 1. Dimensionality Reduction

Dimensionality reduction transforms high-dimensional data into lower-dimensional representations while preserving meaningful information.

Benefits include:

* Easier visualization
* Reduced computational complexity
* Improved interpretability

---

### 2. PCA (Principal Component Analysis)

PCA is a linear dimensionality reduction method.

#### Characteristics
* Preserves global variance
* Computationally efficient
* Works well for linear datasets

#### Limitations
* Cannot capture complex non-linear structures

---

### 3. t-SNE (t-Distributed Stochastic Neighbor Embedding)

t-SNE is a non-linear dimensionality reduction algorithm designed for visualization.

#### Characteristics
* Preserves local neighborhood relationships
* Reveals hidden clusters
* Excellent for visualization of complex datasets

#### Limitations
* Computationally expensive
* Poor preservation of global distances
* Sensitive to hyperparameters

---

### 4. Local vs Global Structure

#### PCA
* Preserves global structure
* Maintains large-scale variance relationships

#### t-SNE
* Preserves local neighborhood structure
* Focuses on cluster formation and nearby points

---

### 5. Computational Complexity

The notebook also explores computational considerations:

* PCA scales efficiently
* t-SNE runtime increases rapidly with dataset size
* High-dimensional datasets increase computational cost

---

## Results and Insights

Key observations from the experiments:

* t-SNE produces clearer cluster separation than PCA
* PCA provides better preservation of global structure
* Non-linear methods reveal hidden manifold structures
* t-SNE is highly effective for visualization tasks
* Hyperparameter tuning strongly affects t-SNE outputs

---

## Applications of t-SNE

t-SNE is widely used in:

* Image Processing
* NLP Embedding Visualization
* Bioinformatics
* Customer Segmentation
* Anomaly Detection
* Deep Learning Feature Visualization

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* Scikit-learn
* Seaborn
* Jupyter Notebook / Google Colab

---

## Conclusion

This lab demonstrates how t-SNE provides powerful visualization capabilities for high-dimensional datasets by preserving local neighborhood relationships. Compared to PCA, t-SNE excels at uncovering hidden clusters and non-linear structures.

Although computationally expensive, t-SNE remains one of the most popular techniques for exploratory data visualization in machine learning.

---

## Author

**Shreya Sari**  
AIML Training Program – Module 2 Lab 04

---

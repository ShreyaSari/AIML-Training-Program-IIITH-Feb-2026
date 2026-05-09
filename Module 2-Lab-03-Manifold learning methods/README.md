# AIML Module 2 – Lab 03

## Manifold Learning Methods

---

## Overview

This notebook explores **manifold learning techniques** used for non-linear dimensionality reduction in machine learning. The primary goal of this lab is to understand how high-dimensional data can be represented in lower-dimensional spaces while preserving meaningful geometric structures.

The notebook focuses on the **ISOMAP algorithm** and compares its behavior with other dimensionality reduction methods such as PCA. The experiments demonstrate how manifold learning helps uncover hidden structures in complex datasets.

---

## Objectives

The main objectives of this lab are:

* Understand the concept of **manifold learning**
* Learn how non-linear dimensionality reduction works
* Explore the working of the **ISOMAP algorithm**
* Compare ISOMAP with PCA
* Analyze the effect of neighborhood size in manifold learning
* Study visualization of high-dimensional datasets in lower dimensions

---

## Dataset

The notebook uses synthetic and/or high-dimensional datasets to visualize manifold structures and dimensionality reduction behavior.

The datasets are transformed into lower-dimensional representations for analysis and visualization.

---

## Key Concepts Covered

### 1. Manifold Learning

Manifold learning assumes that high-dimensional data lies on a lower-dimensional manifold embedded within a higher-dimensional space.

The goal is to uncover this hidden structure while preserving important relationships between data points.

---

### 2. ISOMAP Algorithm

ISOMAP (Isometric Mapping) is a non-linear dimensionality reduction technique that preserves geodesic distances between points on a manifold.

The algorithm involves:

* Constructing a neighborhood graph
* Computing geodesic distances
* Applying multidimensional scaling (MDS)

---

### 3. Neighborhood Graphs

The number of neighbors significantly impacts ISOMAP performance.

#### Low Number of Neighbors
* May disconnect the graph
* Poor manifold reconstruction
* Noisy embeddings

#### High Number of Neighbors
* May distort manifold structure
* Behaves similarly to PCA
* Loses non-linear advantages

---

### 4. PCA vs ISOMAP

#### PCA
* Linear dimensionality reduction method
* Preserves global variance
* Cannot capture curved manifolds effectively

#### ISOMAP
* Non-linear dimensionality reduction method
* Preserves manifold geometry
* Better for complex curved datasets

---

### 5. Other Manifold Learning Methods

The notebook also discusses alternative manifold learning techniques:

* t-SNE
* UMAP
* Locally Linear Embedding (LLE)

These methods differ in how they preserve local and global data structures.

---

### 6. Handling Missing Data

Missing values can affect manifold learning performance because distance calculations become unreliable.

Techniques discussed include:

* Mean/Median Imputation
* KNN Imputation
* Model-Based Imputation
* Matrix Factorization Methods

---

## Results and Insights

Key observations from the experiments:

* ISOMAP performs well on non-linear datasets
* Neighborhood size strongly influences embedding quality
* PCA struggles with curved manifold structures
* Manifold learning preserves hidden geometric relationships
* Visualization becomes more interpretable after dimensionality reduction

---

## Applications of Manifold Learning

Manifold learning techniques are widely used in:

* Image Processing
* Face Recognition
* Data Visualization
* Bioinformatics
* Natural Language Processing
* Recommendation Systems

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook / Google Colab

---

## Conclusion

This lab provides practical exposure to **manifold learning methods** and demonstrates how non-linear dimensionality reduction techniques can uncover hidden structures in high-dimensional datasets.

ISOMAP proves particularly effective when data lies on curved manifolds, while PCA remains useful for simpler linear relationships. Understanding these techniques is important for visualization, feature extraction, and exploratory data analysis in machine learning.

---

## Author

**Shreya Sari**  
AIML Training Program – Module 2 Lab 03

---

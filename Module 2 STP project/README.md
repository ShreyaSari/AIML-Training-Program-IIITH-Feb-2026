# STP Module 2 – Customer Segmentation using Dimensionality Reduction

## Customer Behavior Analysis using PCA, t-SNE, and UMAP

---

## Overview

This notebook explores the application of **dimensionality reduction techniques** for customer segmentation and behavioral analysis in an e-commerce dataset. The project focuses on transforming high-dimensional customer purchasing data into lower-dimensional representations for visualization and business insight generation.

The notebook demonstrates how techniques such as **PCA, t-SNE, and UMAP** help uncover hidden customer patterns, identify behavioral clusters, and support strategic decision-making.

---

## Objectives

The main objectives of this project are:

* Understand the importance of **dimensionality reduction** in data analysis
* Perform **RFM (Recency, Frequency, Monetary)** customer analysis
* Visualize customer behavior using:
  * PCA (Principal Component Analysis)
  * t-SNE (t-Distributed Stochastic Neighbor Embedding)
  * UMAP (Uniform Manifold Approximation and Projection)
* Compare linear and non-linear dimensionality reduction methods
* Extract actionable business insights from customer clusters

---

## Dataset

The dataset used in this notebook contains e-commerce transactional data including customer purchase behavior.

### Features Used

* Customer ID
* Invoice Date
* Quantity Purchased
* Unit Price
* Country
* Purchase Amount

From these features, customer-level RFM metrics are generated.

---

## Key Concepts Covered

### 1. RFM Analysis

RFM analysis is used to measure customer purchasing behavior.

#### Recency (R)
Measures how recently a customer made a purchase.

#### Frequency (F)
Measures how often a customer makes purchases.

#### Monetary (M)
Measures how much money a customer spends.

These metrics help identify customer value and engagement levels.

---

### 2. PCA (Principal Component Analysis)

PCA is a **linear dimensionality reduction** technique used to reduce data dimensions while preserving maximum variance.

The notebook demonstrates:

* Variance preservation
* Feature projection into lower dimensions
* Global structure visualization

---

### 3. t-SNE

t-SNE is a **non-linear dimensionality reduction** technique designed for visualization of complex datasets.

The notebook uses t-SNE to:

* Identify hidden customer clusters
* Capture local neighborhood relationships
* Reveal non-linear customer behavior patterns

---

### 4. UMAP

UMAP is a modern dimensionality reduction technique that preserves both local and global data structure.

The notebook explores:

* Cluster continuity
* Efficient visualization of large datasets
* Improved scalability compared to t-SNE

---

### 5. Data Normalization

Feature normalization ensures all variables contribute equally during dimensionality reduction.

Normalization helps:

* Improve model stability
* Reduce bias from large-scale features
* Enhance clustering performance

---

## Results and Insights

Key observations from the experiments:

* PCA provides a broad overview of customer behavior patterns
* t-SNE reveals highly distinct behavioral clusters
* UMAP balances local and global structure effectively
* High-value customers form dense and identifiable clusters
* Customer behavior is influenced more by purchasing patterns than geography alone
* Dimensionality reduction significantly improves interpretability of high-dimensional customer data

---

## Business Insights

The analysis enables businesses to:

* Identify high-value customers
* Detect churn-risk customers
* Design targeted marketing campaigns
* Improve customer retention strategies
* Build personalized recommendation systems
* Perform region-specific customer analysis

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Plotly
* UMAP-learn
* Jupyter Notebook / Google Colab

---

## Conclusion

This project demonstrates how dimensionality reduction techniques can transform complex customer datasets into meaningful visual insights. PCA, t-SNE, and UMAP each contribute unique advantages for customer segmentation and behavioral analysis.

The results highlight the importance of data visualization in understanding customer patterns, improving business strategies, and supporting data-driven decision-making.

---

## Author

**Shreya Sari**  
STP Training Program – Module 2

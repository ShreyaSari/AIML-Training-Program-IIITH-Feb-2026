# AIML Module 3 – Lab 02  
# Implementing KNN from Scratch and Visualizing Algorithm Performance

## Overview
This notebook explores the implementation of distance metrics and the K-Nearest Neighbors (KNN) algorithm from scratch. The lab focuses on understanding how distance calculations influence classification behavior and how KNN decision boundaries change under different configurations.

The notebook also investigates the impact of high-dimensional data on distance metrics and demonstrates how the “curse of dimensionality” affects neighborhood-based learning algorithms.

---

# Objectives
The main objectives of this lab are:

- Implement Minkowski distance from scratch
- Understand the relationship between Manhattan and Euclidean distance
- Visualize KNN decision boundaries for different K values
- Analyze how distance metrics influence classification
- Study the behavior of distance metrics in high-dimensional spaces
- Understand the curse of dimensionality
- Compare uniform and distance-based KNN weighting methods

---

# Dataset
The notebook uses synthetic and sample datasets for visualization and classification experiments.

The datasets are used to:

- Visualize KNN decision boundaries
- Compare neighborhood relationships
- Analyze the impact of different distance metrics
- Study distance concentration in higher dimensions

---

# Key Concepts Covered

## 1. Minkowski Distance
Minkowski distance is a generalized distance metric defined as:

\[
d(x,x') = \left( \sum_{j=1}^{D} |x_j - x'_j|^p \right)^{1/p}
\]

Special cases include:

- Manhattan Distance when \( p = 1 \)
- Euclidean Distance when \( p = 2 \)

The notebook implements this metric manually using NumPy operations.

---

## 2. K-Nearest Neighbors (KNN)
KNN is a supervised machine learning algorithm used for classification and regression tasks.

The algorithm works by:

- Calculating distances between points
- Finding the nearest neighbors
- Predicting labels based on neighboring samples

The notebook visualizes how KNN behaves with different values of K.

---

## 3. Decision Boundary Visualization
Decision boundaries help visualize how machine learning models separate classes.

The notebook demonstrates:

- Mesh grid creation
- Class prediction over feature space
- Visualization using contour plots
- Effect of changing K values
- Comparison between Euclidean and Manhattan metrics

---

## 4. Curse of Dimensionality
As dimensionality increases:

- Distances between points become less distinguishable
- Neighbor relationships become weaker
- KNN performance may degrade

The notebook analyzes this phenomenon using:

- Euclidean distance
- Manhattan distance
- Chebyshev distance

---

## 5. Distance Metrics in High Dimensions
The notebook compares how different metrics behave as dimensions increase by analyzing:

- Maximum distance
- Minimum distance
- Ratio between max and min distances

This helps understand distance concentration effects.

---

# Results and Insights

Key observations from the experiments:

- Smaller K values create irregular decision boundaries and may overfit
- Larger K values create smoother boundaries and generalize better
- Manhattan distance produces different boundary shapes than Euclidean distance
- High-dimensional data reduces the effectiveness of distance-based learning
- Distance-weighted KNN gives more importance to nearby neighbors

---

# Applications

Distance metrics and KNN are widely used in:

- Recommendation Systems
- Image Classification
- Pattern Recognition
- Medical Diagnosis
- Fraud Detection
- Customer Segmentation
- Anomaly Detection

---

# Technologies Used

- Python
- NumPy
- Matplotlib
- Scikit-learn
- SciPy
- Pandas
- Jupyter Notebook / Google Colab

---

# Conclusion

This lab provides a practical understanding of distance metrics and KNN classification. By implementing Minkowski distance manually and visualizing KNN decision boundaries, we gain insight into how distance calculations influence machine learning behavior.

The experiments on high-dimensional data further demonstrate the challenges posed by the curse of dimensionality and highlight the importance of selecting appropriate distance metrics and model parameters.

Understanding these concepts is essential for building effective neighborhood-based machine learning models.

---

# Author

Shreya Sari  
AIML Training Program – Module 3 Lab 02

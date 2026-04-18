# AIML Module 2 – Lab 02  
## Principal Components Analysis (PCA)

---

## Overview  

This notebook focuses on understanding and implementing **Principal Components Analysis (PCA)**, one of the most important dimensionality reduction techniques used in machine learning and data analysis.

The objective of this lab is to study how high-dimensional data can be transformed into a lower-dimensional space while retaining most of the important information. The notebook demonstrates both the mathematical intuition behind PCA and its practical implementation using Python libraries.

PCA is widely used for:

- Data visualization
- Feature reduction
- Noise removal
- Faster model training

---

## Objectives  

The main objectives of this lab are:

- Understand the concept of Principal Components Analysis (PCA)  
- Learn why dimensionality reduction is important  
- Perform data standardization before PCA  
- Compute covariance matrix, eigenvalues, and eigenvectors  
- Calculate explained variance  
- Reduce the dimensionality of the dataset  
- Visualize the transformed data in 2D and 3D  
- Understand real-world applications of PCA  

---

## Dataset  

The dataset used in this notebook is the **Breast Cancer dataset** from `sklearn.datasets`.

**Dataset Details:**

- **Samples:** 569  
- **Features:** 30 numerical features  
- **Target Labels:**  
  - 0 → Benign  
  - 1 → Malignant  

The features include measurements such as:

- Radius  
- Texture  
- Perimeter  
- Area  
- Smoothness  
- Compactness  

These features help classify tumors as benign or malignant.

---

## Key Concepts Covered  

### 1. Data Standardization  

Before applying PCA, the data is standardized using `StandardScaler`.

This ensures:

- Mean = 0  
- Standard Deviation = 1  

Standardization is important because PCA is highly sensitive to feature scales.

---

### 2. Covariance Matrix  

The covariance matrix is computed to understand how features vary with respect to each other.

This helps identify relationships between variables and is the foundation for computing principal components.

---

### 3. Eigenvalues and Eigenvectors  

PCA uses eigenvalues and eigenvectors of the covariance matrix.

- **Eigenvectors** → directions of maximum variance  
- **Eigenvalues** → amount of variance captured in each direction  

These form the principal components.

---

### 4. Explained Variance  

Explained variance tells us how much information each principal component retains.

This helps determine:

- How many components are needed  
- How much data variance is preserved  

---

### 5. Dimensionality Reduction  

The original 30-dimensional dataset is reduced to:

- 2 dimensions for visualization  
- 3 dimensions for advanced plotting  

This makes the data easier to interpret while retaining important patterns.

---

### 6. Data Visualization  

The notebook includes:

- 2D PCA scatter plot  
- 3D PCA interactive visualization using Plotly  

These plots help visualize the separation between benign and malignant classes.

---

## Results and Insights  

Key observations from the analysis:

- The first few principal components capture most of the variance  
- PCA significantly reduces dimensionality without major information loss  
- The transformed data shows clear separation between the two classes  
- PCA helps improve visualization and can speed up machine learning models  
- Fewer dimensions make the data easier to analyze  

---

## Real-World Applications  

Some common applications of PCA include:

- Image compression  
- Face recognition  
- Feature extraction  
- Noise reduction  
- Data visualization  
- Preprocessing before machine learning  

---

## Technologies Used  

- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Plotly  
- Scikit-learn  
- Jupyter Notebook / Google Colab  

---

## Conclusion  

This lab provides a strong understanding of how PCA works both mathematically and practically. By reducing high-dimensional data into fewer principal components, we can simplify analysis, improve visualization, and make machine learning models more efficient.

PCA is one of the most widely used preprocessing techniques in data science and machine learning.

---

## Author  

**Shreya Sari**  
AIML Training Program – Module 2 Lab 02  

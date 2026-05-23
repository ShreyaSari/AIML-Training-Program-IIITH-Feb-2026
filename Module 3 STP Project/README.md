# AIML Module 3 – Project  
## Exploring and Improving the KNN Classification System

---

## Overview

This project focuses on exploring and improving the performance of the K-Nearest Neighbors (KNN) classification system using the Pima Indians Diabetes Dataset. The project investigates how different preprocessing techniques, feature scaling methods, K-value selection, and feature selection strategies affect the overall accuracy and efficiency of the system.

The project also demonstrates the importance of data visualization and model evaluation techniques in building better machine learning classification systems.

---

## Objectives

The main objectives of this project are:

- Explore the behavior of the KNN classification system
- Improve model performance using preprocessing techniques
- Perform exploratory data analysis (EDA)
- Visualize relationships between features
- Compare unscaled and scaled datasets
- Apply StandardScaler and MinMaxScaler
- Find the optimal K-value for KNN
- Implement K-Fold Cross Validation
- Analyze the impact of feature selection on system performance
- Improve classification accuracy and generalization

---

## Dataset

The project uses the **Pima Indians Diabetes Dataset**.

The dataset contains medical diagnostic information such as:

- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

The target variable:

- **Outcome**
  - 0 → Non-Diabetic
  - 1 → Diabetic

---

## Key Concepts Covered

### 1. Exploratory Data Analysis (EDA)

EDA techniques used in the project include:

- Histograms
- Count plots
- Correlation heatmaps
- Feature distribution analysis
- Statistical summaries

These visualizations help understand feature distributions, correlations, and patterns within the dataset.

---

### 2. K-Nearest Neighbors (KNN)

KNN is a supervised machine learning algorithm used for classification tasks.

The algorithm works by:

- Calculating distances between data points
- Finding the nearest neighbors
- Predicting class labels based on neighboring samples

The project evaluates KNN performance using different K-values ranging from 1 to 40.

---

### 3. Feature Scaling

Since KNN is a distance-based algorithm, feature scaling plays a critical role in improving model performance.

The project compares:

#### StandardScaler
- Transforms data to:
  - Mean = 0
  - Standard Deviation = 1

#### MinMaxScaler
- Scales features between:
  - 0 and 1

#### Unscaled Data
- Original dataset without normalization

The project analyzes which scaling method produces the best accuracy.

---

### 4. K-Fold Cross Validation

The project implements:

- 5-Fold Cross Validation

This helps:

- Reduce overfitting
- Obtain more reliable accuracy estimates
- Analyze model stability using standard deviation

Cross-validation scores are computed for all scaling techniques.

---

### 5. Feature Selection

Feature selection is performed using correlation analysis.

The project:

- Identifies the top features most correlated with the target variable
- Creates reduced feature datasets
- Compares reduced and full feature set performance

The experiments help determine whether fewer features improve or reduce model performance.

---

## Challenge Implementations

### Challenge 1: MinMax Scaling Comparison

Implemented:

- MinMaxScaler preprocessing
- KNN evaluation on MinMax-scaled data
- Comparison between:
  - Unscaled data
  - Standardized data
  - MinMax-scaled data

Insights:
- Scaling improves KNN performance because KNN depends heavily on distance calculations.
- Features with large ranges dominate predictions if scaling is not applied.

---

### Challenge 2: K-Fold Cross Validation Analysis

Implemented:

- 5-Fold Cross Validation
- Accuracy evaluation for K = 1 to 40
- Mean accuracy and standard deviation calculations
- Error bar visualization for model stability analysis

Insights:
- Cross-validation provides more robust performance estimates.
- Lower standard deviation indicates better model consistency.

---

### Challenge 3: Feature Selection and Performance Analysis

Implemented:

- Correlation-based feature selection
- Reduced feature datasets
- Accuracy comparison between:
  - Full feature set
  - Reduced feature set

Bonus:
- Experiments with different numbers of features:
  - 3 Features
  - 5 Features
  - 6 Features

Insights:
- Removing irrelevant features can improve generalization.
- Excessive feature reduction may reduce prediction performance.

---

## Results and Insights

Key observations from the project:

- Feature scaling significantly improves KNN accuracy.
- Standardized and MinMax-scaled data outperform unscaled data.
- Proper K-value selection improves model generalization.
- Cross-validation provides stable and reliable evaluation metrics.
- Feature selection can reduce complexity while maintaining strong accuracy.
- Highly correlated features contribute more to diabetes prediction.

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

---

## Applications

These techniques are widely used in:

- Medical Diagnosis
- Disease Prediction
- Healthcare Analytics
- Fraud Detection
- Recommendation Systems
- Customer Classification
- Pattern Recognition

---

## Conclusion

This project successfully explored and improved the performance of the K-Nearest Neighbors (KNN) classification system using different preprocessing and evaluation techniques.

The experiments demonstrated that feature scaling significantly improves the effectiveness of KNN since the algorithm relies heavily on distance calculations. Both Standardization and MinMax Scaling produced better accuracy compared to unscaled data.

The project also highlighted the importance of selecting an appropriate K-value, applying cross-validation for reliable evaluation, and using feature selection techniques to reduce complexity while maintaining strong predictive performance.

Overall, this project provides practical understanding of how preprocessing, scaling, parameter tuning, and feature analysis contribute to improving machine learning classification systems.

---

## Author

**Shreya Sari**  
AIML Training Program – Module 3 Project

# AIML Module 1 – Lab 2

## Machine Learning Terms and Metrics

### Overview

This notebook explores fundamental machine learning concepts related to **model evaluation, validation strategies, and nearest neighbour classifiers**. The goal of the lab is to understand how different data splitting strategies and evaluation techniques influence the reliability of model performance estimates.

The notebook demonstrates the use of **Nearest Neighbour classifiers**, validation splits, and cross-validation techniques to evaluate model performance on a real dataset.

---

### Objectives

The main objectives of this lab are:

* Understand the importance of **training, validation, and test datasets**
* Learn how **data splitting affects model performance**
* Implement and evaluate **Nearest Neighbour classifiers**
* Compare the behaviour of **1-Nearest Neighbour (1-NN)** and **3-Nearest Neighbour (3-NN)**
* Understand how **cross-validation improves reliability of accuracy estimates**

---

### Dataset

The notebook uses the **California Housing dataset** available in scikit-learn.
For the purpose of this lab, the continuous house price values are converted into **discrete classes**, allowing the problem to be treated as a **classification task instead of regression**.

---

### Key Concepts Covered

#### 1. Dataset Splitting

The dataset is divided into three parts:

* **Training Set** – used to train the model
* **Validation Set** – used to tune and evaluate model performance during development
* **Test Set** – used for final evaluation of the model

This helps prevent overfitting and provides a better estimate of how the model performs on unseen data.

---

#### 2. 1-Nearest Neighbour (1-NN)

The notebook first implements a **1-Nearest Neighbour classifier**, which predicts the label of a data point based on the label of the closest training sample.

Observations from this experiment include:

* Training accuracy tends to be very high
* Validation accuracy is usually lower due to generalization error

---

#### 3. 3-Nearest Neighbour (3-NN)

As part of the exercise, a **3-Nearest Neighbour classifier** is implemented.

Instead of relying on a single neighbour, the classifier:

1. Finds the **three closest training samples**
2. Uses **majority voting** among their labels
3. Assigns the most frequent label as the prediction

This approach generally produces **more stable predictions** compared to 1-NN.

---

#### 4. Cross-Validation

The notebook also explores **cross-validation**, where the dataset is repeatedly split into training and validation sets multiple times.

This helps:

* Reduce randomness caused by a single split
* Provide a **more reliable estimate of model performance**
* Improve confidence in the evaluation results

---

### Results and Insights

Key observations from the experiments:

* Increasing the validation size improves reliability but reduces training data.
* Averaging accuracy across multiple splits produces more consistent results.
* The **3-Nearest Neighbour classifier** tends to be more stable than **1-Nearest Neighbour** because it considers multiple neighbours.
* Cross-validation helps produce a more dependable estimate of model performance.

---

### Technologies Used

* Python
* NumPy
* Scikit-learn
* Jupyter / Google Colab

---

### Conclusion

This lab provides practical insight into how **evaluation strategies affect machine learning models**. By experimenting with different validation splits, nearest neighbour classifiers, and cross-validation techniques, we gain a better understanding of how to obtain **reliable estimates of model performance**.

---

### Author

**Shreya Sari**
AIML Training Program – Module 1 Lab 2

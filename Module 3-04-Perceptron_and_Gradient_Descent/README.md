# AIML Module 3 – Lab 03

## Using K-Nearest Neighbors (KNN) for Text Classification

## Overview

This lab explores the application of the **K-Nearest Neighbors (KNN)** algorithm for text classification using Natural Language Processing (NLP) techniques. The objective is to transform textual data into numerical representations and use KNN to classify documents into predefined categories.

The notebook demonstrates how different text preprocessing and vectorization techniques influence classification accuracy and overall model performance.

---

## Objectives

The primary objectives of this lab are:

* Understand text preprocessing techniques in NLP
* Convert textual data into numerical feature vectors
* Implement text classification using KNN
* Compare Bag-of-Words (BoW) and TF-IDF approaches
* Analyze the impact of feature extraction on model accuracy
* Understand stemming and lemmatization concepts
* Evaluate classification performance using machine learning metrics

---

## Dataset

The notebook utilizes text classification datasets such as:

* Spam Detection Dataset
* Review/Sentiment Dataset

These datasets are used to:

* Classify text into categories
* Train and evaluate KNN models
* Compare vectorization techniques
* Analyze prediction accuracy

---

## Key Concepts Covered

### 1. Text Preprocessing

Text preprocessing is a crucial step in NLP that cleans and standardizes raw text before model training.

The preprocessing pipeline includes:

* Lowercasing text
* Removing punctuation
* Removing stopwords
* Tokenization
* Stemming
* Lemmatization

These techniques help reduce noise and improve model performance.

---

### 2. Bag-of-Words (BoW)

Bag-of-Words is a text representation technique that converts documents into numerical vectors based on word frequency.

#### Process:

1. Build a vocabulary of unique words.
2. Count word occurrences in each document.
3. Represent documents as frequency vectors.

#### Advantages

* Simple to implement
* Computationally efficient

#### Limitations

* Ignores word order
* Does not capture semantic meaning

---

### 3. TF-IDF Vectorization

TF-IDF (Term Frequency – Inverse Document Frequency) improves upon Bag-of-Words by assigning importance scores to words.

#### Formula

```text
TF-IDF = TF × IDF
```

Where:

* **TF** = Frequency of a word in a document
* **IDF** = Importance of the word across all documents

#### Benefits

* Reduces the influence of common words
* Highlights informative and discriminative terms
* Often achieves better classification accuracy than BoW

---

### 4. K-Nearest Neighbors (KNN)

KNN is a supervised machine learning algorithm used for classification.

#### Working Principle

1. Calculate similarity or distance between samples.
2. Identify the K nearest neighbors.
3. Assign the majority class among the neighbors.

#### Impact of K Value

* Smaller K values may lead to overfitting.
* Larger K values provide smoother decision boundaries.
* Selecting an optimal K is important for achieving good performance.

---

### 5. Stemming and Lemmatization

#### Stemming

Reduces words to their root form by removing suffixes.

Examples:

```text
running → run
studies → studi
```

**Advantages**

* Fast
* Computationally inexpensive

**Limitations**

* May produce non-dictionary words

---

#### Lemmatization

Converts words to their dictionary base form while considering context.

Examples:

```text
running → run
better → good
```

**Advantages**

* More accurate
* Preserves semantic meaning

**Limitations**

* Computationally more expensive

---

## Results and Insights

Key observations from the experiments:

* TF-IDF generally outperforms Bag-of-Words.
* Common words contribute less useful information for classification.
* Proper preprocessing improves prediction accuracy.
* Smaller K values may overfit training data.
* Larger K values often provide better generalization.
* Lemmatization preserves semantic meaning better than stemming.

---

## Applications

Text classification and NLP techniques are widely used in:

* Spam Email Detection
* Sentiment Analysis
* Chatbots and Virtual Assistants
* Recommendation Systems
* Search Engines
* Document Categorization
* Fraud Detection
* Social Media Monitoring

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* NLTK
* Jupyter Notebook
* Google Colab

---

## Project Workflow

```text
Text Data
    ↓
Text Preprocessing
    ↓
Feature Extraction
 (BoW / TF-IDF)
    ↓
Train-Test Split
    ↓
KNN Model Training
    ↓
Prediction
    ↓
Performance Evaluation
```

---

## Conclusion

This lab provides practical experience in applying **K-Nearest Neighbors (KNN)** to text classification problems using NLP techniques.

By comparing **Bag-of-Words** and **TF-IDF** vectorization methods, we gain valuable insights into how feature extraction influences machine learning performance. The experiments also highlight the importance of preprocessing techniques such as stemming and lemmatization for improving text quality and classification accuracy.

Understanding these concepts is essential for building efficient NLP systems and real-world text mining applications.

---

## Author

**Shreya Sari**
*AIML Training Program – Module 3 Lab 03*

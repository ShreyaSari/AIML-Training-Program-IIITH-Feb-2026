# AIML Module 3 – Lab 03  
## Using KNN for Text Classification

---

## Overview
This notebook explores the application of the **K-Nearest Neighbors (KNN)** algorithm for **text classification** tasks using Natural Language Processing (NLP) techniques. The lab focuses on converting textual data into numerical feature vectors using **Bag-of-Words (BoW)** and **TF-IDF** representations and then applying the KNN classifier for prediction.

The notebook also investigates how text preprocessing and vectorization methods influence classification accuracy and model performance.

---

## Objectives
The main objectives of this lab are:

- Understand text preprocessing techniques in NLP
- Convert textual data into numerical vectors
- Implement text classification using KNN
- Compare Bag-of-Words and TF-IDF approaches
- Analyze the impact of feature extraction on model accuracy
- Understand stemming and lemmatization concepts
- Evaluate classification performance using machine learning metrics

---

## Dataset
The notebook uses datasets such as:

- **Spam Detection Dataset**
- **Review/Sentiment Dataset**

These datasets are used to:

- Classify text into categories
- Train and test KNN models
- Compare vectorization techniques
- Analyze prediction accuracy

---

## Key Concepts Covered

### 1. Text Preprocessing
Text preprocessing is an important step in NLP that cleans and standardizes raw text data before model training.

The notebook includes preprocessing steps such as:

- Lowercasing text
- Removing punctuation
- Removing stopwords
- Tokenization
- Stemming
- Lemmatization

These steps help improve model performance and reduce noise in the dataset.

---

### 2. Bag-of-Words (BoW)
Bag-of-Words is a simple text representation technique that converts text into frequency vectors.

The process involves:

- Creating a vocabulary of unique words
- Counting the frequency of each word in a document
- Representing documents as numerical vectors

Although simple and efficient, BoW treats all words equally and ignores semantic meaning.

---

### 3. TF-IDF Vectorization
TF-IDF (Term Frequency–Inverse Document Frequency) improves upon BoW by assigning higher importance to meaningful words and reducing the influence of commonly occurring words.

TF-IDF is calculated using:

TF-IDF = TF × IDF

Where:

- **TF** = Frequency of the word in the document
- **IDF** = Importance of the word across all documents

TF-IDF generally provides better accuracy because it highlights discriminative words.

---

### 4. K-Nearest Neighbors (KNN)
KNN is a supervised machine learning algorithm used for classification tasks.

The algorithm works by:

- Calculating similarity/distance between text vectors
- Finding the nearest neighboring documents
- Predicting the class based on nearby samples

Different K values influence model behavior and classification performance.

---

### 5. Stemming and Lemmatization
The notebook also discusses two important NLP normalization techniques:

#### Stemming
- Reduces words to their root form by removing suffixes
- Faster but less accurate
- Example:
  - “running” → “run”
  - “studies” → “studi”

#### Lemmatization
- Converts words into their dictionary base form
- More accurate and context-aware
- Example:
  - “better” → “good”
  - “running” → “run”

---

## Results and Insights

Key observations from the experiments:

- TF-IDF generally performs better than Bag-of-Words
- Common words contribute less useful information for classification
- Proper preprocessing improves prediction accuracy
- Smaller K values may overfit the training data
- Larger K values provide smoother generalization
- Lemmatization preserves semantic meaning better than stemming

---

## Applications
Text classification and NLP techniques are widely used in:

- Spam Email Detection
- Sentiment Analysis
- Chatbots and Virtual Assistants
- Recommendation Systems
- Search Engines
- Document Categorization
- Fraud Detection
- Social Media Monitoring

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- NLTK
- Jupyter Notebook / Google Colab

---

## Conclusion
This lab provides a practical understanding of how KNN can be applied to text classification problems using NLP techniques. By comparing Bag-of-Words and TF-IDF vectorization methods, we gain insight into how feature extraction impacts machine learning performance.

The experiments further demonstrate the importance of preprocessing techniques such as stemming and lemmatization in improving text quality and classification accuracy.

Understanding these concepts is essential for building efficient NLP and text mining applications.

---

## Author
**Shreya Sari**  
AIML Training Program – Module 3 Lab 03

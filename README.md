# Smart Expense Categorizer

A **machine learning-powered application** that automatically categorizes financial transactions based on their descriptions.  
It helps users **analyze spending patterns**, **visualize expenses**, and **gain insights** into their financial behavior.

---

## Project Overview

The **Smart Expense Categorizer** takes a transaction description (e.g., _"Dinner at Domino's"_ or _"Paid electricity bill"_)  
and predicts its expense category — such as **Food**, **Utilities**, **Travel**, **Shopping**, etc.

It uses **Natural Language Processing (NLP)** and **Machine Learning** techniques to learn from historical expense data  
and classify new transactions accurately.

---

## Tech Stack

- **Programming Language:** Python  
- **Libraries Used:**
  - `pandas` — data manipulation and cleaning  
  - `numpy` — numerical operations  
  - `matplotlib`, `seaborn` — data visualization  
  - `scikit-learn` — model building and evaluation  
  - `nltk` — text preprocessing and tokenization  

---

## Project Workflow

### 1. Data Preprocessing
- Clean transaction descriptions (remove punctuation, numbers, stopwords).
- Convert text to lowercase.
- Tokenize and lemmatize text.

### 2. Feature Engineering
- Use **TF-IDF Vectorization** to convert text into numerical features.

### 3. Model Building
- Train a **classification model** (Logistic Regression / SVM / Naive Bayes)  
  to map transaction text → category.

### 4. Model Evaluation
- Evaluate model performance using:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - Confusion Matrix

### 5. Prediction
- Enter a new transaction description to predict its category.

---

## Why Use a Pipeline?

A **Pipeline** in scikit-learn is used to combine preprocessing and model steps  
into a single, reusable object.

Example:
```python
from sklearn.pipeline import Pipeline
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.linear_model import LogisticRegression

model = Pipeline([
    ('tfidf', TfidfVectorizer(stop_words='english')),
    ('clf', LogisticRegression())
])

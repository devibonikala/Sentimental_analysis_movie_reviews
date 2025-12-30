# Sentimental_analysis_movie_reviews
# 🎬 Sentiment Analysis using BoW + TF-IDF + Logistic Regression

This repository contains a simple yet effective *Sentiment Analysis* project built using *scikit-learn*.  
The goal is to classify IMDB movie reviews as *positive* or *negative* using an end-to-end machine learning pipeline.

Only *6 sample reviews* are used from the original dataset to demonstrate the complete workflow clearly.

---

## 📌 Dataset

- *Dataset Name:* IMDB Dataset of 50K Movie Reviews
- *Source:* Kaggle  
- *Link:* https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews
- *Original Size:* 50,000 reviews
- *Used in this project:* 6 reviews (for learning and demonstration)

### Labels
- 1 → Positive Review  
- 0 → Negative Review  

---

## 🧠 Approach & Model

This project uses a *single scikit-learn Pipeline* that combines multiple NLP techniques.

### Pipeline Architecture

Raw Text
├── CountVectorizer (Bag of Words)
├── TfidfVectorizer (TF-IDF)
└── FeatureUnion (concatenation)
↓
Logistic Regression

### Why this approach?
- *Bag of Words (BoW):* Captures raw word frequency
- *TF-IDF:* Reduces importance of common words
- *FeatureUnion:* Combines both feature representations
- *Logistic Regression:* Efficient binary classifier

---

## 🛠️ Technologies Used

- Python
- NumPy
- scikit-learn

---

## 📂 Project Structure

sentiment-analysis/
│
├── sentiment_analysis.py # Main Python script
└── README.md # Project documentation

---


## 📈 Model Evaluation

  The model is evaluated using:
  
  Precision
  
  Recall
  
  F1-score
  
  Confusion Matrix
  
  These metrics are printed after execution using:
  
  classification_report
  
  confusion_matrix

## 🎯 Key Learning Outcomes

  Understanding TF-IDF and BoW
  
  Building end-to-end ML pipelines
  
  Using FeatureUnion
  
  Making predictions with pipeline.predict()
  
  Avoiding feature mismatch and data leakage

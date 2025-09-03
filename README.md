# Sentiment_Analysis_using_EDA_and-ML
🧠 Sentiment and Emotion Analysis on Twitter using Traditional Models

This repository presents a complete pipeline for analyzing public sentiment and emotions from Twitter data. We apply both traditional machine learning models (e.g., Logistic Regression, SVM, Random Forest) to classify tweets based on sentiment (Negative, Neutral, Positive) and emotion (Joy, Sadness, Anger, Optimism).

📂 Dataset Source

This project uses the publicly available Twitter dataset related to the Ukraine–Russia crisis:
- [Ukraine–Russian Crisis Twitter Dataset (1.2M Tweets) — Kaggle](https://www.kaggle.com/datasets/bwandowando/ukraine-russian-crisis-twitter-dataset-1-2-m-rows)

📌 Project Objectives

- Perform exploratory data analysis (EDA) on a large Twitter dataset.

- Engineer custom features like engagement scores and time-based tweet behavior.

- Implement sentiment classification using:

- Rule-based models (TextBlob)

- Machine learning (Logistic Regression, SVM, Random Forest, Decision Trees)

- Perform emotion classification (anger, joy, optimism, sadness) using traditional classifiers.

- Evaluate models using precision, recall, F1-score, accuracy, and confusion matrix.

📂 Dataset Description

Source: Sampled from Twitter API stream

- Size: ~700,000 tweets with 28 attributes

Features:

- User Info: username, acctdesc, location, followers, following, totaltweets

- Tweet Info: text, hashtags, created_at, language

- Engagement: retweetcount, favorite_count

- NLP Targets: Sentiment & Emotion labels

- All tweets were filtered to include only English-language content.

⚙️ Methodology
🔧 Preprocessing

- Lowercasing, URL and mention removal, emoji handling

- Stopword removal using NLTK

- Lemmatization using spaCy

- Custom features: text length, hourly activity, engagement score

📊 Exploratory Data Analysis (EDA)

- Word clouds for frequent terms and sentiment/emotion categories

- Time-series plots (hourly, weekly, monthly)

- Text length distributions vs. engagement levels

🧠 Models Used
## 🧠 Models Used  

| **Task**     | **Traditional Models**                         |  
|--------------|------------------------------------------------|  
| Sentiment    | TextBlob, Logistic Regression, SVM, RF, DT     |  
| Emotion      | Naive Bayes, KNN, Logistic Regression, SVM     |  

📈 Model Evaluation
🔹 Sentiment Classification (Linear SVC)

- Accuracy: 86.7%

- Macro F1-score: 0.86

- Weighted F1-score: 0.87

🔹 Emotion Classification (Linear SVC)

- Accuracy: 85.6%

- Macro F1-score: 0.82

- Best per-class F1:

- Anger: 0.91

- Joy: 0.83

- Optimism: 0.78

- Sadness: 0.76


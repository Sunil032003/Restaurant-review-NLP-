# 🍽️ Restaurant Review Sentiment Analysis using NLP

## 📌 Project Overview

This project performs **Sentiment Analysis** on restaurant customer reviews using **Natural Language Processing (NLP)** and **Machine Learning**. Customer feedback is collected, preprocessed, classified into sentiment categories, and analyzed to identify common service issues. The project also generates insights that can help restaurants improve customer satisfaction.

---

## 🎯 Objectives

* Collect restaurant review data.
* Preprocess customer feedback text.
* Perform sentiment classification.
* Identify common service issues.
* Prepare a customer feedback analysis report.

---

## 📂 Dataset

The dataset contains restaurant reviews with the following attributes:

| Column     | Description               |
| ---------- | ------------------------- |
| Restaurant | Restaurant name           |
| Reviewer   | Reviewer name             |
| Review     | Customer review text      |
| Rating     | Customer rating (1–5)     |
| Metadata   | Reviewer statistics       |
| Time       | Review date and time      |
| Pictures   | Number of uploaded images |

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* NLTK
* Scikit-learn
* Regular Expressions (re)

---

## 🔄 Workflow

1. Load restaurant review dataset.
2. Clean and preprocess review text.
3. Convert text into numerical features using TF-IDF.
4. Create sentiment labels from ratings.
5. Train a Machine Learning model.
6. Predict customer sentiment.
7. Evaluate model performance.
8. Identify common service issues.
9. Generate a feedback analysis report.

---

## 🧹 Text Preprocessing

The following preprocessing steps are applied:

* Convert text to lowercase.
* Remove special characters and punctuation.
* Tokenization.
* Remove stopwords.
* Apply Porter Stemming.
* Create a cleaned review column (`Clean_Review`).

Example:

Original Review:

```
The food was amazing and the service was excellent!
```

Clean Review:

```
food amaz servic excel
```

---

## 📊 Feature Extraction

Text is converted into numerical vectors using:

* TF-IDF (Term Frequency–Inverse Document Frequency)

---

## 🤖 Machine Learning Model

The following classifier is used:

* Multinomial Naive Bayes

Alternative models:

* Logistic Regression
* Linear Support Vector Machine (SVM)

---

## 😀 Sentiment Classes

Ratings are converted into sentiment labels:

| Rating | Sentiment |
| ------ | --------- |
| 4–5    | Positive  |
| 3      | Neutral   |
| 1–2    | Negative  |

---

## 📈 Model Evaluation

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## 🔍 Common Service Issue Identification

Negative customer reviews are analyzed to identify frequently occurring complaint keywords such as:

* Service
* Waiting time
* Food quality
* Staff behaviour
* Price
* Hygiene
* Taste

These insights help restaurants identify areas requiring improvement.

---

## 📋 Feedback Analysis Report

The project generates the following insights:

* Total number of reviews
* Positive, Neutral, and Negative review counts
* Average customer rating
* Restaurant-wise average rating
* Top-rated restaurants
* Lowest-rated restaurants
* Frequently mentioned positive words
* Frequently mentioned complaint keywords

---

## 📁 Project Structure

```
Restaurant-Review-Sentiment-Analysis/
│
├── Dataset/
│   └── Restaurant reviews.csv
│
├── notebooks/
│   └── Restaurant_Sentiment_Analysis.ipynb
│
├── README.md
│
└── requirements.txt
```

---

## 🚀 Future Improvements

* Use BERT or RoBERTa for improved sentiment classification.
* Build an interactive Streamlit dashboard.
* Add aspect-based sentiment analysis.
* Deploy the model as a web application.

---

## 📌 Conclusion

This project demonstrates how Natural Language Processing and Machine Learning can be used to analyze customer feedback, classify sentiment, identify common service issues, and generate meaningful business insights from restaurant reviews.

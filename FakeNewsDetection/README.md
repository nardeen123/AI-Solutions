### 📌 Project Overview
This project focuses on detecting fake news articles using Natural Language Processing (NLP) and machine learning. Given a news dataset, the system classifies articles as either Fake (0) or Real (1) based on their content and titles.
The solution applies preprocessing, feature engineering (TF-IDF), and multiple ML models to achieve high accuracy.

### 🛠️ Data Preprocessing
##### Data cleaning: Removed nulls, duplicates, and empty text rows.
##### Target mapping: Mapped label → Fake = 0, Real = 1.
##### Text & title processing:
Lowercasing
Removing punctuation & stopwords
Tokenization
POS tagging & lemmatization
##### Feature engineering:
Created lemmatized_text and lemmatized_title
Combined into combined_text
Applied TF-IDF vectorization
##### Train-test split: 80% training / 20% testing

### 🤖 Models Used
We implemented and compared multiple models:

📊 Logistic Regression

🌳 Decision Tree

⚡ Passive Aggressive Classifier

🧮 Naïve Bayes

✴️ Support Vector Classifier (SVC)

Each model was evaluated with accuracy, confusion matrix, and classification reports.

### 📊 Results

Logistic Regression → Strong baseline

Passive Aggressive & SVC → High accuracy and good generalization

Naïve Bayes → Fast and effective for text data

Decision Tree → Interpretability but weaker generalization

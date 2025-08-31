### 📌 Project Overview

This project focuses on predicting apartment rent categories using machine learning. We built and compared multiple models to classify rent prices based on apartment features such as location, size, amenities, and more.
The dataset contained 9,000 rows and 21 features, which required extensive preprocessing, feature engineering, and selection to achieve high accuracy.

### 🛠️ Data Preprocessing

Missing values handled with mean, mode, and custom mappings.
Outliers treated using Winsorization.
Categorical features encoded with Label Encoding and feature transformation.
Feature engineering created new variables like:

AvgAreaPrice (based on location bins)

NoOfRooms (bedrooms + bathrooms)

CityStateAvg (average rent by city/state)

Trial (custom engineered feature combining multiple attributes)

Feature selection applied using SelectKBest.

### 🤖 Models Used
We trained and evaluated several models:

🌳 Random Forest → 83% test accuracy

🌲 Decision Tree → improved interpretability but prone to overfitting

🔥 Gradient Boosting → 85% test accuracy

⚡ XGBoost → Best model: 92% test accuracy

📈 SVM → good performance but not top results

👥 KNN → high train accuracy, weak generalization

🧩 Ensemble Methods (Stacking, Voting) → up to 84% test accuracy

### 📊 Results
Best Model: XGBoost

✅ Train Accuracy: 98%

✅ Test Accuracy: 92%

Ensemble learning provided additional robustness.
Confusion matrices were used to validate predictions.

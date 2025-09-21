# 🏢 Apartment Rent Prediction System

## 📌 Project Overview
This project focuses on predicting **apartment rent categories** using machine learning.  
We built and compared multiple models to classify rent prices based on apartment features such as **location, size, amenities**, and more.  

The dataset contained **9,000 rows and 21 features**, requiring extensive preprocessing, feature engineering, and selection to achieve high accuracy.

---

## 🛠️ Data Preprocessing

- **Missing Values**: Handled with mean, mode, and custom mappings.  
- **Outliers**: Treated using Winsorization.  
- **Categorical Features**: Encoded with Label Encoding and feature transformation.  
- **Feature Engineering**: Created new variables such as:  
  - `AvgAreaPrice` (based on location bins)  
  - `NoOfRooms` (bedrooms + bathrooms)  
  - `CityStateAvg` (average rent by city/state)  
  - `Trial` (custom engineered feature combining multiple attributes)  
- **Feature Selection**: Applied using **SelectKBest**.  

---

## 🤖 Models Used

We trained and evaluated several models:  

- 🌳 **Random Forest** → 83% test accuracy  
- 🌲 **Decision Tree** → Improved interpretability but prone to overfitting  
- 🔥 **Gradient Boosting** → 85% test accuracy  
- ⚡ **XGBoost** → Best model: 92% test accuracy  
- 📈 **SVM** → Good performance but not top results  
- 👥 **KNN** → High train accuracy, weak generalization  
- 🧩 **Ensemble Methods** (Stacking, Voting) → Up to 84% test accuracy  

---

## 📊 Results

- **Best Model:** XGBoost  
- ✅ **Train Accuracy:** 98%  
- ✅ **Test Accuracy:** 92%  

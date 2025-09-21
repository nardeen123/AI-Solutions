# 🔍 Fraud Detection Analysis Using Machine Learning and Deep Learning

It focuses on building a **fraud detection system** capable of classifying transactions as **fraudulent or non-fraudulent**.  
The project addresses **imbalanced data challenges**, experiments with multiple machine learning and deep learning models, and integrates **real-time dashboards** for fraud monitoring.  

---

## 📌 Abstract
Fraudulent activities like unauthorized transactions, identity theft, and financial scams cause **billions in financial losses annually**, erode customer trust, and increase operational costs.  
This project develops a **robust fraud detection framework** using **unsupervised anomaly detection** and **deep learning models**, combined with interpretability and visualization techniques.  

Key contributions:
- Tackling **imbalanced datasets** with oversampling (SMOTE), undersampling, and ensemble approaches.  
- Experimentation with both **classical ML algorithms** and **neural networks**.  
- Deployment with **interactive dashboards** for real-time monitoring.  

---

## ⚙️ Methodology

### 🔹 Dataset
- **Source:** Simulated **credit card transaction dataset** from Kaggle.  
- Covers **Jan 2019 – Dec 2020** with 1,000 customers & 800 merchants.  
- Contains both **legitimate** and **fraudulent** activities.  

### 🔹 Preprocessing & EDA
- Handled **class imbalance**.  
- Conducted **temporal and geospatial analysis** of fraud patterns.  
- Feature engineering for transaction behavior.  

### 🔹 Models Implemented

#### 🧠 Machine Learning Models
- **Isolation Forest (IF):** Detect anomalies by isolating outliers.  
- **Local Outlier Factor (LOF):** Identify fraud by density deviation.  
- **DBSCAN:** Cluster transactions, treating anomalies as noise.  

#### 🤖 Deep Learning Models
- **Autoencoders:** Detect fraud via reconstruction error.  
- **One-Class Neural Networks (OC-NN):** Best performing model for anomaly detection.  
- **Deep SVDD:** Learn compact hypersphere of normal data, detect outliers beyond it.  

---

## 📊 Results & Evaluation
- **Best Model:** **One-Class Neural Network (OC-NN)**  
- **Performance:** Highest precision and recall for anomaly detection.  
- **Impact:** Significantly reduced **false negatives**, minimizing financial risks.  

📌 Key insight: **Deep learning models outperform traditional methods** for highly imbalanced fraud datasets.  




# 📝 Forum Discussions Categorization

🎉 This project was developed as part of a **Kaggle competition hosted by our university**,  
where our team achieved a **Top Team ranking** 🥇.  
Competition Link: https://www.kaggle.com/competitions/nn-25-forum-discussions-categorization.

The project focuses on **classifying forum discussion texts** into predefined categories using **Natural Language Processing (NLP)** and **Deep Learning models**.  
It experiments with multiple approaches including RNN-based architectures, Transformers, and ensemble techniques, ultimately achieving strong performance with **RoBERTa + BERT ensembles**.

---

## 📌 Project Overview
- **Goal:** Automatically categorize forum discussions to improve organization, searchability, and user experience.  
- **Dataset:** Forum discussion posts (provided for the Kaggle competition).  
- **Techniques Used:**
  - Text preprocessing & augmentation  
  - Tokenization with Keras `Tokenizer`  
  - Word embeddings (GloVe)  
  - Deep learning models (BiLSTM, GRU, Transformer)  
  - Pretrained Transformer models (BERT, RoBERTa, DistilRoBERTa)  
  - Ensemble methods  

---

## ⚙️ Methodology

### 🔹 Preprocessing
- Text tokenization using **Keras Tokenizer**.  
- Conversion into padded sequences (`maxlen=100`).  
- Out-of-vocabulary words replaced with `<OOV>`.  
- Dataset split into **80% training / 20% validation**, stratified by class labels.  

### 🔹 Word Embedding
- Pre-trained **GloVe embeddings** used.  
- Words not found in GloVe represented by zero vectors.  

### 🔹 Models Implemented
1. **BiLSTM**
   - Tested with and without preprocessing.  
   - Accuracy up to **74%**.  
   
2. **GRU**
   - Similar setup to BiLSTM.  

3. **Transformer-based models**
   - **BERT**  
   - **RoBERTa**  
   - **DistilRoBERTa**  

4. **Ensembles**
   - **RoBERTa + DistilRoBERTa** → Accuracy: ~77.6%  
   - **RoBERTa + BERT** → Accuracy: **78.6%** (best performance)  

---

## 📊 Results
- **Best Model:** RoBERTa + BERT ensemble.  
- **Configuration:**  
  - Learning rate: `0.00002`  
  - Weights: `[1, 0.5]` (RoBERTa, BERT)  
  - Epochs: `4`  
  - Batch size: `32`  
  - Max sequence length: `128`  
- **Final Accuracy:** **78.6%**

---

## 🚀 How to Run

### Prerequisites
- Python 3.8+  
- Install dependencies:
  ```bash
  pip install -r requirements.txt
t

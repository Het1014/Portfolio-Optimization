# Fraud Detection System

This project is about detecting fraudulent credit card transactions using Machine Learning.  
The dataset used is the well-known **Credit Card Fraud Detection dataset from Kaggle**.

---

## 🔍 Problem
Credit card companies face a big challenge: finding fraudulent transactions among millions of normal ones.  
Fraud cases are **very rare** compared to genuine ones, so the dataset is **highly imbalanced**.  
Our goal is to build a system that can **spot frauds as accurately as possible** while keeping false alarms low.

---

## 📂 Project Structure
- **fraud-detection-system.ipynb** → Jupyter Notebook with all the code, explanations, and outputs.

---

## 🛠️ Steps in the Project
1. **Import Libraries**  
   - NumPy, Pandas for data handling  
   - Scikit-learn for ML models and metrics  
   - Imbalanced-learn for handling class imbalance  
   - TensorFlow (if using deep learning)

2. **Load the Dataset**  
   - Credit card transactions data (`creditcard.csv`).  
   - Contains anonymized features and a target column (`Class`) → `1` means fraud, `0` means normal.

3. **Exploratory Data Analysis (EDA)**  
   - Check the distribution of fraud vs non-fraud cases.  
   - Visualize imbalance (frauds are less than 1% of the data).

4. **Data Preprocessing**  
   - Train/test split.  
   - Scaling features.  
   - Handle imbalance using techniques like **SMOTE** (oversampling fraud cases).

5. **Model Training**  
   - Tried different ML models (e.g., Logistic Regression, Random Forest, Neural Networks).  
   - Focus on metrics beyond accuracy (because of imbalance).

6. **Model Evaluation**  
   - Metrics: Precision, Recall, F1-score, ROC-AUC.  
   - Emphasis on **Recall for fraud class** (catching frauds is more important).  

---

## 📊 Results
- Models can detect fraud with good **recall and ROC-AUC**.  
- Handling imbalance (SMOTE, undersampling, or weighted models) improves fraud detection significantly.  
- Best models balance between **catching frauds** and **not flagging too many normal transactions**.

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/fraud-detection-system.git
   cd fraud-detection-system

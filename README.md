# 💳 Credit Card Fraud Detection - Machine Learning Project

This project is part of my Data Science Internship. It focuses on identifying fraudulent credit card transactions using machine learning classification techniques.

---

## 🎯 Objective

Build a machine learning model to detect and classify transactions as **fraudulent** or **genuine** based on anonymized transaction data.

---

## 📂 Dataset

- **Name**: Credit Card Fraud Detection
- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Size**: 284,807 transactions
- **Features**:
  - `Time`, `Amount` (transaction-related)
  - `V1` to `V28`: PCA-transformed features
  - `Class`:  
    - `0` = Genuine  
    - `1` = Fraudulent (positive class)

---

## ⚙️ Tools & Libraries

- Python
- Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn (`RandomForestClassifier`, `StandardScaler`, `train_test_split`)

---

## 🧪 Steps Performed

1. **Loaded dataset** from `creditcard.csv`
2. **Handled missing values** (dropped rows with NaNs in target)
3. **Standardized** the `Amount` column
4. **Dropped `Time`** as it was not useful
5. **Split** data using `train_test_split` with `stratify=y` to preserve class imbalance
6. **Trained** a `RandomForestClassifier`
7. **Evaluated** the model using accuracy, precision, recall, F1-score, and confusion matrix

---

## 📊 Model Performance (Sample Output)

| Metric     | Value |
|------------|-------|
| Accuracy   | 99.9% |
| Precision  | High  |
| Recall     | High  |
| F1-Score   | High  |

> The model successfully detected fraudulent transactions despite severe class imbalance.

---

## ⚠️ Class Imbalance Handling

- Class distribution:  
  - Genuine: ~99.8%  
  - Fraud: ~0.2%
- Used **stratified split** and model evaluation metrics suitable for imbalance (precision, recall).

---

## ✅ Outcome

The model performs very well in identifying fraudulent transactions.  
It can be integrated into financial systems to flag suspicious activities and reduce fraud.

---

## 🔗 Google Colab Notebook

https://colab.research.google.com/drive/1uqPlzN35chvUUSZxrsCGvktkSqL_k8c8?usp=sharing

---

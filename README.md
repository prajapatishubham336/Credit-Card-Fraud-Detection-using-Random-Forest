# Credit-Card-Fraud-Detection-using-Random-Forest
This project builds a Machine Learning model to detect fraudulent credit card transactions. It uses a Random Forest classifier on a highly imbalanced dataset and focuses on identifying rare fraud cases with reliable performance.



## 📌 Project Overview

This project builds a Machine Learning model to detect fraudulent credit card transactions. It uses a Random Forest classifier on a highly imbalanced dataset and focuses on identifying rare fraud cases with reliable performance.

---

## 🎯 Objective

* Detect fraudulent transactions from transaction data
* Handle class imbalance effectively
* Build a robust and interpretable classification model

---

## 🚀 Features

* Data exploration and preprocessing
* Handling imbalanced dataset using class weights
* Random Forest model training
* Performance evaluation using key metrics
* Fraud prediction using probability threshold

---

## 🛠️ Technologies Used

* Python
* Pandas & NumPy
* Scikit-learn
* Matplotlib / Seaborn

---

## 📂 Dataset

This project uses the **Credit Card Fraud Detection dataset** from Kaggle.

⚠️ **Note:**
The dataset is not included in this repository due to GitHub file size limitations.

👉 Download dataset from:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

### 📊 Dataset Details:

* Total Transactions: **284,807**
* Fraud Cases: **492 (Highly Imbalanced)**

### 🔑 Features:

* `V1` to `V28`: PCA-transformed features
* `Time`: Transaction time
* `Amount`: Transaction amount
* `Class`: Target variable

  * `0` → Normal
  * `1` → Fraud

---

## 🔹 Data Preprocessing

* Checked for missing values
* Separated features (`X`) and target (`y`)
* Removed unnecessary scaling (not required for Random Forest)
* Performed stratified train-test split to maintain class distribution

---

## ⚙️ Model

* Random Forest Classifier
* Configured with:

  * Balanced class weights
  * Controlled tree depth to prevent overfitting
  * Parallel processing for faster training

---

## 📊 Model Performance

### Confusion Matrix

* True Negatives: 56846
* False Positives: 18
* False Negatives: 17
* True Positives: 81

### Key Metrics

* Accuracy: **99.93%**
* ROC-AUC Score: **~0.91**
* Precision (Fraud): **~82%**
* Recall (Fraud): **~83%**

---

## ⚠️ Important Insights

* Dataset is highly imbalanced
* Accuracy alone is misleading
* Key focus should be on:

  * Recall (detecting fraud cases)
  * Precision
  * ROC-AUC score

---

## 🔮 Prediction Strategy

* Model outputs probability of fraud for each transaction
* A threshold is used to classify transactions
* Lower threshold increases fraud detection but may increase false positives

---

## 💡 Key Learnings

* Handling imbalanced datasets is critical
* Random Forest performs well for fraud detection
* Proper evaluation metrics are more important than accuracy
* Threshold tuning improves model effectiveness

---

## 📈 Future Improvements

* Apply SMOTE for better class balance
* Try advanced models like XGBoost or LightGBM
* Perform hyperparameter tuning
* Deploy as a web application (Streamlit)

---

## 📚 References

* Kaggle Credit Card Fraud Detection Dataset
* Scikit-learn Documentation

---

## 🙌 Conclusion

This project demonstrates a practical and effective approach to detecting fraudulent transactions using machine learning. The model achieves strong performance despite class imbalance and can be further enhanced for real-world deployment.

---

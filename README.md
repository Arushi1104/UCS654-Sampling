# 📊 Probabilistic Sampling Methods – Model Performance Comparison

## 📌 Overview
This project is based on the **Credit Card Fraud Detection dataset**, where the goal is to classify transactions as:

- **Class = 0 → Normal**
- **Class = 1 → Fraud**

Since the dataset is **imbalanced**, applying sampling methods is important to improve model learning and fair evaluation.

---

## 🎯 Objective
The main objectives of this assignment are:

- ✅ Balance the dataset to handle class imbalance  
- ✅ Apply **probabilistic sampling techniques**  
- ✅ Train multiple ML models on each sample  
- ✅ Compare accuracy and identify the best sampling method for each model  

---

## 📂 Dataset Information

| Feature | Details |
|--------|---------|
| Dataset | Creditcard_data.csv |
| Target Column | `Class` |
| Task Type | Binary Classification |
| Major Challenge | Imbalanced Dataset |

---

## ✅ Probabilistic Sampling Techniques Used

| Sampling Method | Short Explanation |
|----------------|------------------|
| **Simple Random Sampling** | Randomly selects records (equal chance) |
| **Systematic Sampling** | Selects every k-th record |
| **Stratified Sampling** | Maintains class proportion in sample |
| **Cluster Sampling** | Divides into groups, selects clusters randomly |
| **Bootstrap Sampling** | Sampling with replacement |

---

## 🤖 Models Used

- Logistic Regression  
- Decision Tree  
- Random Forest  
- KNN  
- SVM  

---

## 📊 Accuracy Results (%)

The table below shows accuracy scores of each model trained using each sampling method:

| Model | Simple Random Sampling | Systematic Sampling | Stratified Sampling | Cluster Sampling | Bootstrap Sampling |
|------|------------------------:|--------------------:|-------------------:|----------------:|------------------:|
| **Logistic Regression** | 93.44 | 92.35 | 92.35 | 93.44 | **93.99** |
| **Decision Tree** | 97.27 | 96.72 | 94.54 | 97.54 | **98.36** |
| **Random Forest** | **99.45** | **99.45** | **99.45** | 99.18 | **99.45** |
| **KNN** | 90.16 | 95.63 | 90.71 | **95.90** | 95.08 |
| **SVM** | 97.27 | 98.91 | 97.81 | 97.54 | **99.45** |

---

## 🏆 Best Sampling Method for Each Model

| Model | Best Sampling Method | Best Accuracy (%) |
|------|-----------------------|------------------:|
| Logistic Regression | **Bootstrap Sampling** | **93.99** |
| Decision Tree | **Bootstrap Sampling** | **98.36** |
| Random Forest | **Simple Random Sampling** | **99.45** |
| KNN | **Cluster Sampling** | **95.90** |
| SVM | **Bootstrap Sampling** | **99.45** |

---

## 🔍 Key Observations
- **Bootstrap Sampling** gave the best results for most models (Logistic Regression, Decision Tree, and SVM).
- **Random Forest** achieved the highest overall accuracy (**99.45%**) and performed consistently across multiple sampling methods.
- **KNN** performed better with **Systematic Sampling** and **Cluster Sampling** compared to Simple Random and Stratified sampling.
- **Stratified Sampling** produced lower accuracy for Decision Tree and KNN in this experiment.

---

## ✅ Final Conclusion
This assignment shows that **sampling method selection impacts model performance**.

- 🏆 **Best Overall Model:** **Random Forest (99.45%)**
- 🥇 **Best Overall Sampling Method:** **Bootstrap Sampling** (best for 3 out of 5 models)

Choosing the right combination of **Sampling Technique + Machine Learning Model** helps improve fraud detection performance.

---

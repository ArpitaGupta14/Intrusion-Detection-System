# 🚨 Intrusion Detection System for IoT (ML-Based)

## 📌 Project Overview

This project presents a **Machine Learning–based Intrusion Detection System (IDS)** designed to detect and classify cyberattacks in **IoT and network environments** using the **UNSW-NB15 dataset**. The system supports both **binary classification (Normal vs Attack)** and **multiclass classification (9 attack categories)** with high accuracy.

The project focuses on handling **realistic network traffic**, **class imbalance**, and **complex attack patterns** using ensemble learning techniques, with **XGBoost** as the primary optimized model.


---

## 🎯 Objectives

* Detect malicious network traffic effectively in IoT environments
* Handle **severely imbalanced attack classes** using SMOTE
* Compare traditional and ensemble ML models
* Achieve high accuracy for both binary and multiclass intrusion detection

---

## 🧠 Key Features

* End-to-end **ML pipeline** (preprocessing → training → evaluation)
* Supports **Binary & Multiclass Intrusion Detection**
* **SMOTE-based imbalance handling** for rare attack types
* Model comparison: Logistic Regression, Random Forest, XGBoost
* Detailed evaluation using Accuracy, Precision, Recall, F1-score, and Confusion Matrix

---

## 📊 Dataset

* **Dataset Used:** UNSW-NB15
* **Source:** Australian Centre for Cyber Security (ACCS)
* **Attack Types:** DoS, Exploits, Reconnaissance, Shellcode, Backdoor, Worms, etc.
* **Labels:**

  * `label` → Binary classification (Normal / Attack)
  * `attack_cat` → Multiclass attack category


---

## ⚙️ Methodology

1. **Data Acquisition**

   * Loaded and merged UNSW-NB15 CSV files

2. **Data Preprocessing**

   * Missing value handling
   * Categorical feature encoding
   * Feature normalization
   * Class imbalance correction using **SMOTE**

3. **Model Training**

   * Logistic Regression (baseline)
   * Random Forest
   * Optimized XGBoost (tuned hyperparameters)

4. **Evaluation**

   * Accuracy
   * Precision, Recall, F1-score
   * Confusion Matrix
   * Feature Importance analysis

---

## 🏆 Results

| Task                      | Best Model | Accuracy   |
| ------------------------- | ---------- | ---------- |
| Binary Classification     | XGBoost    | **99.2%**  |
| Multiclass Classification | XGBoost    | **84.24%** |

XGBoost consistently outperformed Logistic Regression and Random Forest by learning **nonlinear attack patterns** and improving detection of minority attack classes.


---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Libraries:** Scikit-learn, XGBoost, Pandas, NumPy, Matplotlib
* **Techniques:** Machine Learning, Ensemble Learning, SMOTE, Feature Engineering
* **Domain:** Cybersecurity, IoT Security

---

## 📂 Project Structure

```
├── data/
│   └── UNSW-NB15 dataset
├── preprocessing/
│   └── data_cleaning.py
├── models/
│   ├── logistic_regression.py
│   ├── random_forest.py
│   └── xgboost_model.py
├── evaluation/
│   └── metrics.py
├── README.md
```

---

## 🚀 Future Enhancements

* Integration of **Deep Learning models (CNN, RNN, Transformers)**
* Real-time IDS deployment for IoT & cloud environments
* Feature selection using GA, PCA, or mutual information
* Cross-dataset validation (CICIDS2017, Bot-IoT)

---.

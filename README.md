# 📧 SmartInbox

A machine learning-based spam detection system that classifies messages as **Spam** or **Ham (legitimate)** using **TF-IDF feature extraction** and **Logistic Regression**.

The project focuses on building a reliable text-classification pipeline with proper train/validation/test separation, hyperparameter tuning, and error analysis.

---

## 🚀 Features

- 📩 Binary classification of messages into **Spam** and **Ham**
- 🔤 TF-IDF-based text representation
- 🔢 1–4 gram features to capture word and phrase patterns
- 🤖 Logistic Regression classifier
- 🎯 Hyperparameter tuning using validation data
- 🔒 Leakage-free train/validation/test pipeline
- 📊 Test-set performance evaluation
- 🔍 Qualitative error analysis of misclassified messages

---

## 📈 Results

The final model achieved:

**97.58% test accuracy**

on a dataset containing **73K+ messages**.

| Model | Features | Test Accuracy |
|-------|----------|---------------|
| TF-IDF + Logistic Regression | 1–4 grams | **97.58%** |

---

## 🧠 Approach

The overall pipeline is:

```text
Raw Messages
     │
     ▼
Text Preprocessing
     │
     ▼
Train / Validation / Test Split
     │
     ▼
TF-IDF Vectorization
     │
     ▼
Logistic Regression
     │
     ▼
Hyperparameter Tuning
     │
     ▼
Final Model
     │
     ▼
Test Evaluation
     │
     ▼
Error Analysis

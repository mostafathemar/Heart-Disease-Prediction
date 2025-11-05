# ❤️ Heart Disease Prediction (Cardiology – Core Simulation)

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1b-A8QPkgNjtqrq_aTMrPj73uSi5RnAp9?usp=drive_link)

---

## 📘 Overview

This project predicts **the presence of heart disease** in patients using several **machine learning algorithms** and advanced optimization techniques.  
It demonstrates how AI can **detect cardiovascular risks early**, helping to design **AI-assisted clinical trials** and improve preventive healthcare.

The dataset comes from the **UCI Cleveland Heart Disease repository (303 patients)** and includes demographic and clinical features such as age, blood pressure, cholesterol, and chest pain type.

---

## 🎯 Project Goal

- Build an **AI model** to predict heart disease presence  
- Compare multiple ML algorithms and tuning strategies  
- Demonstrate how **AI-driven simulations** can identify high-risk patients and improve **clinical trial efficiency**

---

## ⚙️ Methodology

### **1. Data Preprocessing**
- Cleaned missing values and normalized numeric features  
- Handled outliers and categorical encoding  

### **2. Exploratory Data Analysis (EDA)**
- Visualized feature correlations and distributions  
- Identified top predictors (cholesterol, chest pain, oldpeak)

### **3. Feature Selection**
- Selected most relevant features using statistical importance scores  

### **4. Model Training & Optimization**
- Trained **7 algorithms**:
  - Logistic Regression  
  - Random Forest  
  - Decision Tree  
  - SVM  
  - Naive Bayes  
  - KNN  
  - Extra Trees (Ensemble)
- Used **Optuna** and **GridSearchCV** for hyperparameter optimization

---

## 📊 Results

| Model | Accuracy | Optimization |
|-------|-----------|--------------|
| **Extra Trees** | **98.8%** | Optuna |
| Random Forest | 98.0% | GridSearch |
| Logistic Regression | 86% | GridSearch |
| SVM | 70% | GridSearch |
| KNN | 76% | K-min tuning |
| Decision Tree | 84% | GridSearch |
| XGBoost | 82% | GridSearch |
| AdaBoost | 83% | GridSearch |

✅ The **Extra Trees Classifier (Optuna)** achieved the **best performance** — 98.8% accuracy, with near-perfect precision and recall.

---

## 💡 Clinical Value

- Enables **early detection** of heart disease risk  
- Supports **Synthetic Control Arm** design in clinical trials  
- Reduces costs by up to **50%** by predicting control outcomes  
- Helps in patient stratification for personalized medicine  

---

## 🧠 Tools & Technologies

`Python`, `Scikit-learn`, `Optuna`, `Matplotlib`, `Seaborn`, `Pandas`, `NumPy`

---


---

## 🧭 Usage

**Google Colab (no setup required):**  
[🔗 Run in Colab](https://colab.research.google.com/drive/1b-A8QPkgNjtqrq_aTMrPj73uSi5RnAp9?usp=drive_link)

**Local Setup:**
```bash
git clone https://github.com/mostafathemar/Heart-Disease-Prediction.git
cd Heart-Disease-Prediction
pip install -r requirements.txt
jupyter notebook heart_disease.ipynb

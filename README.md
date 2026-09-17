# 🚀 Customer Churn & Retention Analysis (Data Science & Machine Learning)

An end-to-end, beginner-friendly data science project designed to analyze customer turnover, predict churn using machine learning, and provide actionable business retention strategies.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AsemaniJoshua/Retention-Analysis-Data-Science-Project/blob/main/telco_customer_churn_analysis.ipynb)
![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Dataset](https://img.shields.io/badge/Dataset-IBM%20Telco%20Churn-orange.svg)
![Status](https://img.shields.io/badge/Progress-All%208%20Sections%20Completed-brightgreen.svg)

---

## 📌 Project Overview
- **Problem**: Predict whether a subscription customer will cancel service and identify which factors drive turnover.
- **Dataset**: IBM Telco Customer Churn (7,043 customer records, 21 feature columns).
- **Core Methodology**:
  1. Exploratory Data Analysis (EDA) & Business Storytelling
  2. Missing Value Imputation & Data Type Conversion
  3. Categorical Encoding (Binary & One-Hot Encoding)
  4. Class Imbalance Mitigation (SMOTE vs. Cost-Sensitive Class Weights)
  5. Predictive Modeling (Logistic Regression, Random Forest, XGBoost)
  6. Evaluation with Precision-Recall and ROC-AUC Curves
  7. Feature Importance & Executive Retention Recommendations

---

## 📂 Project Structure
- [`telco_customer_churn_analysis.ipynb`](file:///c:/Users/JOSHUA%20ASEMANI/Music/Data%20Science/Retention-Analysis-Data-Science-Project/telco_customer_churn_analysis.ipynb): The master Jupyter Notebook containing all 8 step-by-step sections, ELI5 explanations, and pre-computed outputs.
- [`README.md`](file:///c:/Users/JOSHUA%20ASEMANI/Music/Data%20Science/Retention-Analysis-Data-Science-Project/README.md): Project overview and curriculum guide.

---

## 🧭 Step-by-Step Curriculum
- [x] **Section 1: Setup, Ingestion & Initial Detective Work**
- [x] **Section 2: Data Cleaning & Column Dictionary (Child-Friendly Guide)**
- [x] **Section 3: Exploratory Data Analysis (EDA) & Storytelling Visualizations**
- [x] **Section 4: Feature Engineering & Preprocessing Pipeline**
- [x] **Section 5: Handling Class Imbalance (SMOTE vs. Class Weights)**
- [x] **Section 6: Model Training & Head-to-Head Comparison**
- [x] **Section 7: Model Evaluation & The ROC-AUC Curve**
- [x] **Section 8: Feature Importance, Retention Strategies & Business Impact**

---

## 🏆 Final Results & Key Takeaways

| Metric / Analysis | Result | Business Interpretation |
| :--- | :---: | :--- |
| **Model Recall** | **85.25%** | Catches the vast majority of churning customers (vs. 0% for dummy baseline). |
| **ROC-AUC Score** | **0.8484** | Outstanding discriminative ability to rank customers from highest to lowest churn risk. |
| **Top Predictors** | `Contract`, `Fiber Optic`, `Tenure`, `Tech Support` | Long-term contracts and tech support anchor retention; expensive month-to-month fiber drives churn. |
| **Net Annual ROI** | **$153,154+ (481.6% ROI)** | Saving just 15% of identified churners yields massive recurring enterprise value. |
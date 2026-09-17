# 🚀 Customer Churn & Retention Analysis (Data Science & Machine Learning)

An end-to-end, beginner-friendly data science project designed to analyze customer turnover, predict churn using machine learning, and provide actionable business retention strategies.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AsemaniJoshua/Retention-Analysis-Data-Science-Project/blob/main/telco_customer_churn_analysis.ipynb)
![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Dataset](https://img.shields.io/badge/Dataset-IBM%20Telco%20Churn-orange.svg)
![Status](https://img.shields.io/badge/Progress-Complete%20%26%20Production--Ready-brightgreen.svg)

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
  8. **Model Serialization & Deployment**: Saving artifacts to `models/` for instant sub-millisecond production inference!

---

## 📂 Project Structure
- [`telco_customer_churn_analysis.ipynb`](file:///c:/Users/JOSHUA%20ASEMANI/Music/Data%20Science/Retention-Analysis-Data-Science-Project/telco_customer_churn_analysis.ipynb): The master Jupyter Notebook containing all 8 foundational sections + Bonus Section 9, ELI5 explanations, and pre-computed outputs.
- [`models/`](file:///c:/Users/JOSHUA%20ASEMANI/Music/Data%20Science/Retention-Analysis-Data-Science-Project/models/): Production-ready serialized model artifacts:
  - [`models/best_churn_model.joblib`](file:///c:/Users/JOSHUA%20ASEMANI/Music/Data%20Science/Retention-Analysis-Data-Science-Project/models/best_churn_model.joblib): Serialized champion classifier.
  - [`models/customer_scaler.joblib`](file:///c:/Users/JOSHUA%20ASEMANI/Music/Data%20Science/Retention-Analysis-Data-Science-Project/models/customer_scaler.joblib): Fitted `StandardScaler` normalization ruler.
  - [`models/model_features.json`](file:///c:/Users/JOSHUA%20ASEMANI/Music/Data%20Science/Retention-Analysis-Data-Science-Project/models/model_features.json): Exact ordered list of 30 feature names.
  - [`models/README.md`](file:///c:/Users/JOSHUA%20ASEMANI/Music/Data%20Science/Retention-Analysis-Data-Science-Project/models/README.md): Quick-start instructions for loading and predicting in production.
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
- [x] **Bonus Section 9: Model Persistence & Instant Single-Customer Prediction Engine**

---

## 🏆 Final Results & Key Takeaways

| Metric / Analysis | Result | Business Interpretation |
| :--- | :---: | :--- |
| **Model Recall** | **85.25%** | Catches the vast majority of churning customers (vs. 0% for dummy baseline). |
| **ROC-AUC Score** | **0.8484** | Outstanding discriminative ability to rank customers from highest to lowest churn risk. |
| **Top Predictors** | `Contract`, `Fiber Optic`, `Tenure`, `Tech Support` | Long-term contracts and tech support anchor retention; expensive month-to-month fiber drives churn. |
| **Net Annual ROI** | **$153,154+ (481.6% ROI)** | Saving just 15% of identified churners yields massive recurring enterprise value. |
| **Inference Speed** | **< 15 milliseconds** | Instant real-time prediction using serialized `.joblib` model artifacts. |
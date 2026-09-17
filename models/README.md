# 📦 Serialized Production Model Artifacts

This directory contains the production-ready serialized models and preprocessors for the **Telco Customer Churn & Retention Analysis** project.

---

## 📂 Artifact Files

| File | Type | Description | Size |
| :--- | :---: | :--- | :---: |
| **`best_churn_model.joblib`** | Binary Model | The champion trained machine learning classifier with optimized decision weights. | ~174 KB |
| **`customer_scaler.joblib`** | Preprocessor | The `StandardScaler` normalization ruler for continuous features (`tenure`, `MonthlyCharges`, `TotalCharges`). | ~1 KB |
| **`model_features.json`** | JSON Config | The exact ordered list of all 30 feature names expected by the model. | ~1 KB |

---

## ⚡ How to Load & Predict in 3 Lines of Python

You can deploy these models into any backend API (e.g. FastAPI, Flask, Django, Streamlit, or AWS Lambda) without retraining:

```python
import joblib
import json
import pandas as pd

# 1. Load the pre-trained brain and ruler (takes ~10 milliseconds)
scaler = joblib.load("models/customer_scaler.joblib")
model = joblib.load("models/best_churn_model.joblib")
with open("models/model_features.json", "r") as f:
    features = json.load(f)

# 2. Prepare incoming customer data (example: Alice)
customer_df = pd.DataFrame([{
    'tenure': 2,
    'MonthlyCharges': 95.50,
    'TotalCharges': 191.00,
    # ... dummy columns aligned to 'features'
}])
customer_df[['tenure', 'MonthlyCharges', 'TotalCharges']] = scaler.transform(customer_df[['tenure', 'MonthlyCharges', 'TotalCharges']])

# 3. Predict churn risk instantly!
churn_probability = model.predict_proba(customer_df)[0, 1] * 100
print(f"Customer Churn Probability: {churn_probability:.1f}%")
```

---

## 🎯 Actionable Risk Thresholds

- **$\ge$ 70.0%**: 🚨 **High Danger** $\rightarrow$ Dispatch retention specialist call + rate lock discount.
- **40.0% – 69.9%**: ⚠️ **Medium Risk** $\rightarrow$ Proactive email outreach + free tech support upgrade.
- **$<$ 40.0%**: 🌟 **Safe & Loyal** $\rightarrow$ Automated anniversary thank-you message.

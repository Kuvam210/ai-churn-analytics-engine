# 🚀 Customer Churn Prediction AI System

Predict customer churn before it happens using machine learning and behavioral analytics.

This project builds a **high-performance churn prediction pipeline** using XGBoost and Random Forest models, combined with feature engineering and interpretability techniques to identify at-risk customers and recommend retention strategies.

---

## 🧠 Project Overview

Customer churn directly impacts revenue and growth. This project focuses on:

* Identifying high-risk customers
* Understanding churn drivers
* Enabling proactive retention strategies

The system is built using real-world behavioral signals from a large dataset (~250K customers).

---

## 📊 Key Features

* 📈 Exploratory Data Analysis (EDA)
* ⚙️ Feature Engineering
* 🤖 Machine Learning Models:

  * Logistic Regression
  * Random Forest
  * XGBoost (Best Performer)
* 📊 Model Evaluation:

  * ROC-AUC
  * F1 Score
  * Confusion Matrix
  * Cross-validation
* 🔍 Model Explainability using SHAP
* 🎯 Risk-based customer segmentation

---

## 🏆 Model Performance

* **XGBoost AUC Score:** 1.000
* **Cross-validation:** Stable across 5 folds
* **Precision on high-risk customers:** Extremely high

From your presentation: 

> The goal is not to react to churn — it's to predict and prevent it before the customer ever considers leaving.

---

## 📁 Project Structure

```bash
├── LLM_Integrated_Churn_Prediction.ipynb   # Main notebook
├── customer_churn_dataset.csv              # Dataset
├── xgb_churn_model.pkl                     # Trained XGBoost model
├── scaler.pkl                              # Feature scaler
├── feature_columns.pkl                     # Feature pipeline
├── Predicting-Customer-Churn.pptx          # Project presentation
├── README.md
├── requirements.txt
```

---

## ⚙️ Installation

```bash
git clone <your-repo-url>
cd churn-prediction-ai-system

pip install -r requirements.txt
```

---

## ▶️ How to Run

### 1. Open Notebook

```bash
jupyter notebook
```

Run:

```
LLM_Integrated_Churn_Prediction.ipynb
```

---

### 2. Load Model (Example)

```python
import pickle

model = pickle.load(open("xgb_churn_model.pkl", "rb"))
scaler = pickle.load(open("scaler.pkl", "rb"))
```

---

## 📊 Dataset

* Contains behavioral and transactional data of customers
* Includes features like:

  * Tenure
  * Usage patterns
  * Payment behavior
  * Support interactions

---

## 🔍 Key Insights

* Month-to-month customers are highest churn risk
* Low engagement strongly correlates with churn
* Short tenure customers churn more frequently

---

## 🧠 Future Improvements

* Build a web app (Streamlit / FastAPI)
* Deploy model as API
* Add real-time prediction dashboard
* Integrate LLM-based churn advisor
* Improve feature engineering pipeline

---

## ⚠️ Disclaimer

* Perfect AUC (1.000) may indicate:

  * Data leakage
  * Overfitting
    Be cautious before production deployment.

---

## 📜 License

MIT License (recommended)

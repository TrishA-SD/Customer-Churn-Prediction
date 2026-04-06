# 📉 Customer Churn Prediction

A machine learning classification project to predict whether a customer will churn (leave the company) based on their usage patterns and account information.

---

## 📌 Problem Statement

Customer churn is a major concern for businesses in telecom, banking, and SaaS. Losing customers leads to revenue loss and increased acquisition costs. This project builds and compares multiple ML classification models to predict churn using customer data.

---

## 📁 Dataset

- **Source:** Telecom customer dataset
- **Size:** 7,043 rows × 21 columns
- **Target:** `Churn` (Yes / No)

**Key Features:**
| Feature | Description |
|---|---|
| `tenure` | Number of months with the company |
| `MonthlyCharges` | Monthly billing amount |
| `TotalCharges` | Total amount charged |
| `Contract` | Month-to-month / One year / Two year |
| `InternetService` | DSL / Fiber optic / No |
| `PaymentMethod` | Electronic check / Mailed check / Bank transfer / Credit card |

---

## 🔧 Project Pipeline
---

## 🤖 Models Trained

| Model | Accuracy | Recall | F1 Score | ROC-AUC |
|---|---|---|---|---|
| Logistic Regression | 76.5% | 78.0% | 0.637 | 0.850 |
| KNN (k=7) | 71.7% | 80.4% | 0.601 | 0.804 |
| Decision Tree | 72.5% | 65.4% | 0.558 | 0.668 |
| Random Forest | 78.3% | 74.0% | 0.643 | 0.836 |
| Gradient Boosting | 77.8% | 71.8% | 0.631 | 0.853 |
| XGBoost | 77.9% | 69.2% | 0.623 | 0.828 |
| **SVC (Tuned) ✅** | **77.0%** | **79.4%** | **0.646** | **0.851** |

> **Best Model: SVC (Tuned)** — best balance of Recall, F1 Score, and ROC-AUC.

---

## 💡 Key Insight

> **Monthly Charges** is the most important feature for predicting churn. Customers with higher monthly bills are significantly more likely to leave.

---

## 🛠️ Tech Stack

- **Language:** Python 3.x
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn, imbalanced-learn, xgboost

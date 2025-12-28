# Task 2: Customer Churn Prediction

## 📖 Project Overview
This task focuses on building a **machine learning model to predict customer churn** using a structured telecom dataset.  
The objective is to **identify customers likely to churn** so that proactive retention strategies can be applied.

The project follows a **complete ML pipeline**, including preprocessing, model comparison, hyperparameter tuning, and handling class imbalance.

---

## 📊 Dataset Information
- **Dataset Size:** 7,043 rows × 21 columns
- **Target Variable:** `Churn` (Yes / No)
- **Feature Types:**
  - Numerical: `tenure`, `MonthlyCharges`, `SeniorCitizen`
  - Categorical: Contract type, payment method, service subscriptions, etc.

---

## 🧠 Approach & Methodology

### 1. Data Preprocessing
- Used **ColumnTransformer** to handle mixed data types
- Numerical features:
  - Median imputation
  - Standard scaling
- Categorical features:
  - Most frequent imputation
  - One-hot encoding (`handle_unknown='ignore'`)

### 2. Models Implemented
- Logistic Regression (baseline)
- Random Forest Classifier
- Tuned Random Forest (GridSearchCV)
- Logistic Regression with **class weighting**

### 3. Model Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

**Primary metric:** Recall (Churn = Yes)  
**Reason:** Missing churn customers is more costly than false positives.

---

## 🏆 Final Model Selection

**Final Model:** Logistic Regression (Class Weighted)

### Final Performance:
- **Recall (Churn = Yes):** 0.76
- **F1-score:** 0.62
- **Accuracy:** 0.75

This model significantly reduces missed churn customers while maintaining reasonable precision.

---

## 📈 Key Insight
Handling class imbalance using class weighting improved churn detection substantially, making the model more aligned with real-world business objectives.

---

## 🗂 Project Structure
task-2-customer-churn/
│
├── churn_pipeline.ipynb
├── README.md
├── requirements.txt


---

## ▶ How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
jupyter notebook churn_pipeline.ipynb

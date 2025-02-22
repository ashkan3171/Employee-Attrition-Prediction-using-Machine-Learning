# 🚀 Employee Attrition Prediction using Machine Learning

## 📌 Project Overview
Employee attrition is a critical issue for businesses, affecting productivity, morale, and costs. This project builds a machine learning model to predict **which employees are likely to leave**, helping organizations take proactive measures.

## 📊 Dataset
- **Source:** IBM HR Analytics Employee Attrition Dataset
- **Rows:** 1,470 employees
- **Columns:** 35 features (numerical & categorical)
- **Target Variable:** `Attrition` (Yes/No → Converted to 1/0)

## 🔬 Exploratory Data Analysis (EDA)
- Checked class imbalance (**16% employees left, 84% stayed**).
- Identified **key features impacting attrition** (e.g., Job Level, Income, Overtime, Work Experience).
- Visualized correlations between attrition and job-related factors.

## 🛠️ Machine Learning Models Used
✅ **Logistic Regression** (With Class Weighting)  
✅ **Random Forest** (With Class Weighting & SMOTE)  
✅ **XGBoost** (With Hyperparameter Tuning & Decision Threshold Adjustment)

## 🔄 Techniques Implemented
- **One-Hot Encoding & Label Encoding** for categorical variables.
- **Class Imbalance Handling** using **Class Weights & SMOTE**.
- **Feature Scaling** with **StandardScaler** for numerical features.
- **Hyperparameter Tuning** for improved accuracy.
- **Feature Importance Analysis** to optimize model performance.
- **Threshold Tuning** for better recall of `Attrition = 1`.

## 🎯 Best Model Performance (XGBoost)
| Metric | Stayed (`Attrition=0`) | Left (`Attrition=1`) |
|---------|----------------|----------------|
| **Precision** | 0.90 | 0.40 |
| **Recall** | 0.86 | 0.49 |
| **F1-score** | 0.88 | 0.44 |

**Final Model:** XGBoost **with Class Weighting, SMOTE, and Hyperparameter Tuning.**  
We focused on **maximizing recall for `Attrition = 1`** to identify employees at risk of leaving.

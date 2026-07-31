# 📊 Customer Churn Prediction

An end-to-end Machine Learning project that predicts customer churn for a telecommunications company and identifies the key business factors associated with customer retention.

---

## 📌 Project Overview

Customer churn is one of the biggest challenges for subscription-based businesses. Losing existing customers directly impacts revenue and increases customer acquisition costs.

The objective of this project is to:

* Analyze customer behavior and churn patterns.
* Identify the major factors influencing customer churn.
* Build machine learning models to predict whether a customer is likely to churn.
* Provide actionable business recommendations to improve customer retention.

---

## 🎯 Business Problem

A telecommunications company wants to identify customers who are at risk of leaving before they actually churn.

By predicting churn early, the company can:

* Launch targeted retention campaigns.
* Improve customer satisfaction.
* Reduce revenue loss.
* Allocate retention budgets more effectively.

---

## 📂 Dataset

**Dataset:** Telco Customer Churn Dataset

The dataset contains information about customer demographics, subscribed services, billing details, contract information, and whether the customer churned.

### Dataset Summary

* Customers: **7,032**
* Features: **20**
* Target Variable: **Churn**

---

# 🛠️ Project Workflow

## 1. Business Understanding

* Defined the business problem.
* Identified stakeholders.
* Formulated analytical questions.
* Established project objectives.

---

## 2. Data Cleaning

* Removed missing values.
* Corrected data types.
* Converted `TotalCharges` to numeric.
* Removed incomplete customer records.
* Saved a cleaned dataset for downstream analysis.

---

## 3. Exploratory Data Analysis (EDA)

Performed business-focused analysis to answer questions such as:

* Which customers churn the most?
* Does contract type influence churn?
* Does tenure affect customer retention?
* Are monthly charges associated with churn?
* Which payment methods have the highest churn?
* Does Tech Support reduce churn?
* Which customer characteristics are associated with churn?

---

## 4. Machine Learning

Implemented a complete Scikit-learn pipeline including:

* Train-Test Split
* One-Hot Encoding
* Feature Scaling
* Logistic Regression
* Decision Tree
* Random Forest

---

# 📈 Model Performance

| Model               |   Accuracy |  Precision |     Recall |   F1 Score |    ROC-AUC |
| ------------------- | ---------: | ---------: | ---------: | ---------: | ---------: |
| Logistic Regression | **80.38%** | **64.85%** | **57.22%** | **60.80%** | **83.59%** |
| Decision Tree       |     78.96% |     60.21% | **61.50%** | **60.85%** |     82.96% |
| Random Forest       |     78.96% |     63.45% |     49.20% |     55.42% |     81.40% |

### Final Model

**Logistic Regression** was selected as the final model because it achieved:

* Highest Accuracy
* Highest Precision
* Highest ROC-AUC
* Strong overall balance between performance and interpretability

---

# 🔍 Key Insights

The analysis revealed that customer churn is strongly associated with:

* Short customer tenure
* Month-to-month contracts
* Fiber optic internet service
* Higher monthly charges during exploratory analysis
* Electronic check payment method
* Lack of Tech Support

Customers who were least likely to churn generally had:

* Longer tenure
* Two-year contracts
* Tech Support
* Partners and dependents
* Lower-risk internet service plans

---

# 💼 Business Recommendations

Based on the analysis, the company should:

* Encourage customers to switch from month-to-month to long-term contracts.
* Improve onboarding and engagement during the first few months of a customer's journey.
* Investigate why Fiber Optic customers experience higher churn.
* Promote Tech Support adoption through bundled plans or free trials.
* Create targeted retention campaigns for customers predicted to have a high churn probability.
* Review the experience of customers using electronic check payments.

---

# 🧰 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

# 📁 Project Structure

```
Customer-Churn-Prediction/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_Business_Understanding.ipynb
│   ├── 02_Data_Preparation.ipynb
│   ├── 03_Exploratory_Data_Analysis.ipynb
│   └── 04_Machine_Learning.ipynb
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

# 🚀 Future Improvements

Potential enhancements for this project include:

* Hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
* Cross-validation for more robust model evaluation.
* Handling class imbalance using SMOTE or class weighting.
* Explainability using SHAP values.
* Deploying the model as a web application using Streamlit or Flask.
* Monitoring model performance on new customer data.

---

# 👤 Author

**Kunaal Sahu**

Aspiring Data Analyst | Python | SQL | Machine Learning | Business Analytics

This project is part of my Data Analytics & Machine Learning Portfolio, demonstrating an end-to-end workflow from business understanding to predictive modeling and actionable business insights.

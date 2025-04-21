# 🧠 Customer Churn Prediction Model

Welcome to the repository for the **Customer Churn** project. This machine learning model helps us predict whether a customer will leave or stay at a bank based on input parameters such as customer demographics, account information, and service usage.

---

## 📌 Project Overview

- **Problem Statement:**  
  The goal is to predict customer churn—whether a customer will leave the bank—so that the bank can take proactive measures to improve customer retention.

- **Dataset:**  
  The dataset can be accessed [here](https://docs.google.com/spreadsheets/d/1oFX_X_4Mey_r_aH5g8pjtE3asH30e5Z1/edit?usp=drive_link&ouid=111319374470519749129&rtpof=true&sd=true). It contains information about customers' demographics, account details, and service usage. The target variable is whether the customer will leave (churn) or stay.

- **Goal:**  
  The goal of this project is to accurately predict customer churn, which will enable banks to reduce churn by focusing on customers who are likely to leave.

---

## 🚀 Model Details

- **Algorithms Tried**  
  The following models were evaluated:
  - Decision Tree
  - Random Forest
  - K-Nearest Neighbors (KNN)
  - Logistic Regression

  Among these, KNN initially performed better. Multiple values of **k** were tested using accuracy scores, but the results remained unsatisfactory.

- **Final Model Used**  
  `AdaBoost Classifier`  
  AdaBoost was selected for its improved predictive performance and ability to highlight **feature importance**, helping identify which input variables most influenced customer churn.

- **Libraries & Tools**  
  - `numpy`  
  - `pandas`  
  - `matplotlib`  
  - `seaborn`  
  - `scikit-learn`  
  - `imblearn`

- **Performance Metrics**  
  - **Accuracy:** 82.7%  
  - **F1 Score:** 0.57

---

## 🔑 Feature Importance

Using the **AdaBoost Classifier**, we analyzed the feature importance scores to identify which features most influenced customer churn predictions. The top contributing features, based on their importance, are as follows:

- **Age (25.29%)**: Customers ranging from **30 to 40 years old** contribute the most to churn prediction, suggesting that this age group is more likely to leave the bank.
- **Balance (10.81%)**: Account balance plays a significant role in predicting churn. Customers with lower balances tend to be more likely to churn, possibly due to dissatisfaction with services or insufficient funds.
- **Estimated Salary (10.76%)**: The estimated salary of customers impacts churn, with higher earnings correlating to greater customer loyalty.
- **Credit Score (9.87%)**: **Credit score** is a key factor in predicting churn, as customers with lower credit scores are more likely to leave. It indicates financial instability, which might influence their satisfaction with the bank's services.

These insights can help the bank prioritize retention strategies focusing on customers within the 30-40 age range, with low balances, and those with poor credit scores.

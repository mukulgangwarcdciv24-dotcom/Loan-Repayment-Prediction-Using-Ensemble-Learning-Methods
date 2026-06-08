# Loan Repayment Prediction Using Ensemble Learning Methods

## Overview

This project focuses on predicting whether a borrower will fully repay a loan using various Machine Learning and Ensemble Learning techniques. Financial institutions face significant risks when approving loans, and accurate repayment prediction can help reduce defaults and improve lending decisions.

The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, hyperparameter tuning, and comparative evaluation of multiple machine learning algorithms to identify the most effective model for loan repayment prediction.

---

## Problem Statement

Loan defaults can lead to significant financial losses for banks and lending institutions. Therefore, assessing a borrower's repayment capability before approving a loan is crucial.

The objective of this project is to develop a machine learning model that predicts whether a borrower is likely to repay a loan based on their financial and credit-related characteristics.

---

## Dataset

The dataset contains borrower information such as:

- Credit Policy Status
- Loan Purpose
- Interest Rate
- Installment Amount
- Annual Income
- Debt-to-Income Ratio
- FICO Credit Score
- Credit Inquiries in the Last 6 Months
- Revolving Balance
- Revolving Utilization Rate
- Public Records

### Target Variable

| Value | Description |
|---------|---------|
| 0 | Loan Fully Repaid |
| 1 | Loan Not Fully Repaid |

---

## Project Workflow

### 1. Data Preprocessing

- Loaded and explored the dataset using Pandas.
- Checked for missing values and inconsistencies.
- Encoded categorical variables.
- Performed train-test splitting.
- Prepared the dataset for machine learning models.

### 2. Exploratory Data Analysis (EDA)

Various visualizations were created to understand data distribution and feature relationships:

- FICO Score Distribution
- Loan Purpose Analysis
- Interest Rate Analysis
- Credit Policy Comparison
- Correlation Heatmap
- Repayment Trend Analysis

These analyses helped identify important factors influencing loan repayment behavior.

---

## Machine Learning Models Implemented

### Decision Tree Classifier

A Decision Tree model was trained and optimized using GridSearchCV to improve predictive performance.

**Accuracy:** 84.58%

### Bagging Classifier

Bagging was applied using Decision Trees as base estimators to reduce variance and improve model stability.

**Cross-Validation Score:** 73.10%

### AdaBoost Classifier

AdaBoost was implemented to enhance predictive capability by combining multiple weak learners.

**Accuracy:** ~84%

### Random Forest Classifier

Random Forest combines multiple Decision Trees and aggregates their predictions for improved robustness and generalization.

**Accuracy:** 84.70%

### Gradient Boosting Classifier

Gradient Boosting was trained to sequentially correct prediction errors and improve overall model performance.

**Performance:** Comparable to other ensemble learning methods.

---

## Model Comparison

| Model | Accuracy |
|---------|---------|
| Decision Tree | 84.58% |
| Bagging Classifier | 73.10% |
| AdaBoost | ~84% |
| Random Forest | **84.70%** |
| Gradient Boosting | Comparable |

### Best Performing Model

**Random Forest Classifier**

Reasons for selection:

- Highest accuracy among tested models
- Better generalization performance
- Reduced overfitting risk
- Effective handling of complex feature interactions

---

## Technologies Used

### Programming Language

- Python

### Libraries

- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn

### Machine Learning Techniques

- Decision Tree
- Bagging
- AdaBoost
- Random Forest
- Gradient Boosting
- GridSearchCV
- Cross Validation

---

## Evaluation Metrics

The models were evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report
- Precision
- Recall
- F1 Score
- Cross-Validation Score

---

## Key Findings

- Ensemble learning methods significantly improve prediction reliability.
- FICO Score plays a major role in determining repayment likelihood.
- Interest Rate and Credit Policy strongly influence loan outcomes.
- Random Forest achieved the most balanced and accurate performance among all tested models.

---

## Future Improvements

- Feature Selection Techniques
- Hyperparameter Optimization
- XGBoost and LightGBM Implementation
- Class Imbalance Handling
- Model Deployment using Flask or FastAPI
- Real-Time Loan Risk Assessment Dashboard

---

## Repository Structure

```text
├── Loan_Repayment_Prediction.ipynb
├── loan_data.csv
├── README.md
└── requirements.txt
```

---

## Conclusion

This project demonstrates the application of machine learning and ensemble learning techniques for loan repayment prediction. Multiple classification models were evaluated, with the Random Forest Classifier achieving the best overall performance at approximately **84.7% accuracy**.

The results highlight the effectiveness of ensemble learning in credit risk assessment and demonstrate how predictive analytics can support better lending decisions while minimizing financial risk for institutions.

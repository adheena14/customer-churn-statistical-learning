# Customer Churn Prediction & Retention Strategy Using Statistical Learning

Status: Completed

## Overview
This project builds a data-driven customer churn prediction pipeline using statistical learning techniques to identify customers who are likely to leave a service.
The focus is on:
- Understanding key churn drivers
- Building a predictive model
- Translating insights into business actions

## Objectives
- Analyze customer behavior and service attributes related to churn
- Identify high-risk customer segments through exploratory data analysis
- Build a predictive churn model using Logistic Regression
- Evaluate model performance using appropriate classification metrics

## Dataset
- Telecom customer data with demographics, service usage, contract, and billing details
= Target variable: Churn (Yes / No)

## Exploratory Data Analysis (EDA)
Key analyses performed:
- Contract Type vs Churn : Month-to-month contracts show significantly higher churn rates
- Tenure vs Churn : Customers with shorter tenure are more likely to churn
- Monthly Charges vs Churn : Higher monthly charges correlate with increased churn probability
- Payment Method vs Churn : Electronic check users exhibit higher churn
- Gender vs Churn : Minimal impact observed 
EDA findings were used to guide feature selection and business interpretation.

## Data Preprocessing
- Handled missing and invalid numeric values
- Converted monetary and tenure fields to numeric format
- Encoded categorical variables using one-hot encoding
- Scaled numeric features using StandardScaler
- Ensured no data leakage during train-test split

## Modeling Approach
Model used: Logistic Regression
Reason for choice:
          -Strong baseline for classification
          -Interpretability
          -Suitable for business-oriented churn problems

## Model Performance
- #### Accuracy: 79%
- #### ROC-AUC: 0.84

## Business Takeaways
- Focus retention efforts on short-tenure, month-to-month customers
- Review pricing strategies for customers with high monthly charges
- Improve billing experience for high-risk payment methods
- Use model outputs to prioritize customers for proactive engagement

## Tools
Python | Pandas | NumPy | Scikit-learn | Matplotlib | Seaborn

## Author
#### Adheena Jose
M.Tech – Data Science, AI & ML
Aspiring Data Scientist

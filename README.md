# Customer Churn Prediction System


(Note: Some notebooks may not render fully on NBViewer due to size/plot outputs. 
Please use Google Colab or download the notebook to view the complete analysis:

Open in Colab:
 https://colab.research.google.com/github/adheena14/customer-churn-statistical-learning/blob/main/notebooks/Summarynotebook.ipynb

 https://colab.research.google.com/github/adheena14/customer-churn-statistical-learning/blob/main/notebooks/churn_eda.ipynb

)


## Overview
Customer churn is a critical business problem where retaining existing customers is often more cost-effective than acquiring new ones.
This project builds a data-driven customer churn prediction system using machine learning to identify customers who are likely to stop using a service, enabling proactive retention strategies.

## Problem Statement
To predict whether a customer will churn based on historical behavioral and demographic data, and evaluate model performance using industry-standard classification metrics.

## Approach
The project follows an end-to-end machine learning pipeline:
- Data Understanding & Cleaning
- Handled missing values and inconsistent data
- Performed exploratory data analysis (EDA) to identify churn patterns
- Feature Engineering
- Encoded categorical variables
- Scaled numerical features where required
- Selected relevant features influencing churn behavior
- Model Building
- Trained supervised classification models
- Optimized model performance using evaluation metrics
- Model Evaluation
- Precision, Recall, F1-score
- ROC-AUC for overall discriminatory power

## Results
- ROC-AUC: 0.84
- Precision (Churn class): 0.63
- Recall (Churn class): 0.54
These results indicate the model’s ability to effectively distinguish between churned and non-churned customers while maintaining a balance between false positives and false negatives.

## Tech Stack
- Python
- pandas, numpy
- scikit-learn
- matplotlib / seaborn

## Key Learnings
- Importance of evaluation metrics beyond accuracy in imbalanced datasets
- Translating model outputs into actionable business insights
- End-to-end ML workflow from raw data to performance evaluation

## Future Improvements
- Handle class imbalance using advanced techniques (SMOTE, class weighting)
- Hyperparameter tuning for improved recall
- Deployment as a web application or API
- Integration of explainability tools (SHAP / feature importance)

# Customer Churn Prediction & Retention Strategy Using Statistical Learning

Status: Completed (2026-01-13)

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Preprocessing](#data-preprocessing)
- [Modeling Approach](#modeling-approach)
- [Model Performance](#model-performance)
- [Business Takeaways](#business-takeaways)
- [Repository Structure](#repository-structure)
- [Reproducibility & Environment](#reproducibility--environment)
- [How to Contribute](#how-to-contribute)
- [License](#license)
- [Author / Contact](#author--contact)

## Overview
This project builds a data-driven customer churn prediction pipeline using statistical learning techniques to identify customers who are likely to leave a service. The focus is on:
- Understanding key churn drivers
- Building an interpretable predictive model
- Translating insights into actionable retention strategies

## Dataset
- Telecom customer dataset with demographics, service usage, contract, and billing details.
- Target variable: Churn (Yes / No)
- Dataset source: [add link or file location here — e.g., `data/telecom_churn.csv` or a public dataset URL`]

Suggested information to include here:
- Number of rows and columns
- Class balance (percent churn vs. not churn)
- Any filters or exclusions applied

## Exploratory Data Analysis (EDA)
Key analyses performed (high-level summary):
- Contract Type vs Churn: Month-to-month contracts show significantly higher churn rates.
- Tenure vs Churn: Customers with shorter tenure are more likely to churn.
- Monthly Charges vs Churn: Higher monthly charges correlate with increased churn probability.
- Payment Method vs Churn: Electronic check users exhibit higher churn.
- Gender vs Churn: Minimal impact observed.

Visuals: include example plots (histograms, bar charts, correlation heatmap, churn-rate by segment) in `notebooks/figures` or the notebook output.

## Data Preprocessing
High-level steps:
- Handled missing and invalid numeric values (specify strategy: drop / median mean imputation / other).
- Converted monetary and tenure fields to numeric format.
- Encoded categorical variables using one-hot encoding (specify columns and whether rare categories were grouped).
- Scaled numeric features using `StandardScaler`.
- Ensured no data leakage: train-test split performed before scaling and encoding (specify split ratio and random seed).

Recommended details to document:
- Train/test split ratio (e.g., 80/20) and random seed used.
- Imputation method per feature.
- Any feature engineering (e.g., tenure groups, interaction terms).
- Treatment of class imbalance (if applicable): oversampling, undersampling, or `class_weight`.

## Modeling Approach
Model used: Logistic Regression

Why logistic regression:
- Strong baseline for binary classification
- Highly interpretable (feature coefficients)
- Suitable for business-oriented churn problems where probability scores matter

Modeling details to include:
- Regularization type and strength (e.g., L2, C parameter)
- Hyperparameter tuning approach (grid search / randomized CV) and cross-validation strategy
- Whether class weights were used
- Final model training procedure and saved model location (e.g., `models/logistic_model.pkl`)

## Model Performance
- Accuracy: 79% (reported at default threshold 0.5)
- ROC-AUC: 0.84

Recommended additions:
- Precision, recall, F1-score for both classes
- Confusion matrix
- Per-class metrics or a classification report
- Cross-validated scores or standard deviations
- Calibration and threshold analysis (if you will use probabilities to rank customers for retention)

Example metrics section (replace placeholders with actual values):
- Precision (churn): X.XX
- Recall (churn): X.XX
- F1-score (churn): X.XX
- ROC-AUC: 0.84

## Business Takeaways
- Focus retention efforts on short-tenure, month-to-month customers.
- Review pricing and offers for customers with high monthly charges.
- Improve billing experience for customers using electronic check payment methods.
- Use model outputs (probabilities) to prioritize customers for proactive engagement and tailored retention offers.

Operational suggestions:
- Define a retention action policy with expected uplift and estimated cost per contacted customer.
- Run A/B tests on targeted retention campaigns to measure ROI.

## Repository Structure
(Example — update to match your repo)
- notebooks/                - EDA and analysis notebooks
- data/                     - raw and processed datasets (or links)
- src/                      - preprocessing, training, evaluation scripts
- models/                   - saved model artifacts
- figures/                  - plots used in README/notebooks
- requirements.txt
- README.md

## Reproducibility & Environment
- Python version: 3.x (specify exact version)
- Key package versions: Pandas X.X, scikit-learn X.X, numpy X.X, matplotlib X.X
- Random seed used: 42 (or whichever you used)
- Steps to reproduce experiments: (link to notebook and script)

## How to Contribute
- Open an issue for bug reports, feature requests, or questions.
- Create pull requests for code or documentation improvements.
- Add unit tests for important preprocessing and modeling functions (if applicable).

## License
Specify a license (e.g., MIT, Apache-2.0) or add `LICENSE` file. Example:
```
This project is licensed under the MIT License - see the LICENSE file for details.
```

## Author / Contact
Adheena Jose  
M.Tech – Data Science, AI & ML  
GitHub: [adheena14](https://github.com/adheena14)  
Email: [adheenajose1@gmail.com]

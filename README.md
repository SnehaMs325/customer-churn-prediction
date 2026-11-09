# Customer Churn Prediction Using Random Forest

## Project Overview
This project predicts customer churn using machine learning. The goal is to identify telecom customers who may leave the company and support customer retention strategies.

## Dataset
* **Source:** IBM Telco Customer Churn dataset
* **Customers:** 7,043
* **Target:** Churn (Yes/No)
* **Input Features:** 19

## Technologies Used
Python, Pandas, NumPy, Matplotlib, Scikit-learn, Joblib, Jupyter Notebook

## Project Workflow
1. Data cleaning and exploratory data analysis
2. Feature preprocessing using StandardScaler and OneHotEncoder
3. Stratified train/test split (80/20)
4. Logistic Regression and Random Forest model comparison
5. Hyperparameter tuning using RandomizedSearchCV
6. Model evaluation and feature importance analysis
7. Model serialization using Joblib

## Model Performance
**Selected Model:** Tuned Random Forest Classifier

| Metric | Score |
| :--- | :--- |
| Accuracy | 77.15% |
| Churn Precision | 55.28% |
| Churn Recall | 72.73% |
| Churn F1-score | 62.82% |
| Best Cross-Validation F1 | 62.87% |

## Key Findings
* Customer tenure was the most important feature.
* Total charges and month-to-month contracts were strong predictive signals.
* Hyperparameter tuning improved churn recall from 63.10% to 72.73%.
* The tuned model correctly identified 272 of 374 churned customers in the test set.

## Conclusion
The tuned Random Forest model demonstrated useful performance in identifying customers at risk of churn. Future improvements could include validation-based threshold optimization, additional feature engineering, and model explainability techniques.
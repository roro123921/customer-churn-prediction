# Customer Churn Prediction Using Machine Learning

A machine learning project that predicts customer churn and identifies key factors influencing customer retention using customer behaviour and service data.

## Overview

Customer churn is a major challenge for businesses, particularly in industries such as banking and telecommunications where retaining existing customers is more cost-effective than acquiring new ones.

This project develops a machine learning model to predict customers who are likely to leave a service. The goal is to identify key factors contributing to churn and provide insights that businesses can use to improve customer retention strategies.

---

## Business Problem

Customer churn directly impacts revenue and long-term customer relationships.

The objective of this project is to:

- Predict whether a customer is likely to churn.
- Identify the most important factors influencing churn.
- Provide actionable insights to support customer retention strategies.

This project simulates a real-world analytics workflow used by organisations to improve customer experience and reduce customer loss.

---

## Dataset

Dataset:
Customer Churn Prediction Dataset

Source:
[Insert dataset source]

Description:

The dataset contains customer demographic, account, service usage and behavioural information.

Key features include:

- Customer demographics
- Account information
- Contract details
- Payment methods
- Service usage
- Customer satisfaction metrics
- Complaint history

Target variable:

- Churn (Yes/No)

---

## Technologies Used

Programming:
- Python

Libraries:
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

Machine Learning:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting (optional)

Development:
- Jupyter Notebook
- Git/GitHub

---

## Project Workflow

### 1. Data Preparation

Tasks completed:

- Loaded and inspected raw dataset
- Checked missing values
- Removed duplicate records
- Converted data types
- Encoded categorical variables
- Selected relevant features
- Split data into training and testing datasets

---

### 2. Exploratory Data Analysis

Analysed:

- Customer churn distribution
- Relationship between customer characteristics and churn
- Contract type and churn behaviour
- Payment methods
- Customer satisfaction trends

Visualisations include:

- Churn distribution charts
- Feature comparisons
- Correlation analysis

---

### 3. Machine Learning Modelling

Models developed:

| Model | Purpose |
|---|---|
| Logistic Regression | Baseline classification model |
| Decision Tree | Interpretable decision rules |
| Random Forest | Ensemble learning model |
| Gradient Boosting | Improved predictive performance |

Evaluation metrics:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

---

## Results

(Add after completing)

Example:

The Random Forest model achieved the strongest overall performance, identifying customers at higher risk of churn.

Key findings:

- Customers with shorter contract periods had higher churn rates.
- Customer satisfaction was strongly associated with churn behaviour.
- Service engagement was an important predictor of retention.

---

## Business Recommendations

Based on model insights:

- Target high-risk customers with personalised retention offers.
- Improve customer support experiences for dissatisfied customers.
- Encourage longer-term contracts through incentives.
- Monitor customer behaviour changes indicating churn risk.

---

## Future Improvements

Potential improvements:

- Hyperparameter tuning
- Deployment using Flask/Streamlit
- Real-time churn prediction pipeline
- Explainable AI techniques such as SHAP
- Testing on real banking customer datasets

---

## Author

Rohan Sajeesh

Bachelor of Applied Data Science  
Monash University

GitHub:
https://github.com/roro123921

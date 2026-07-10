# Dataset

## Overview

This project uses the **Customer Churn Prediction Dataset_1M** from Kaggle.

The dataset contains **1,000,000 synthetic telecommunications customer records** designed to simulate real-world customer behaviour and churn patterns.

The raw dataset contains:

- 1,000,000 rows
- 32 columns
- Customer demographic information
- Account information
- Service usage data
- Customer behaviour metrics
- Churn outcome

After preprocessing, the final modelling dataset contains:

- 1,000,000 rows
- 31 columns

---

# Raw Dataset

The raw dataset contains customer information before preprocessing.

Example structure:

| customer_id | signup_date | age | gender | annual_income | education | marital_status | dependents | tenure | contract | ... | credit_score | churn |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| CUST0000000001 | 2022-12-12 12:53:58 | 43 | Female | 55085.25 | college | married | 1 | 2 | two_year | ... | NaN | 0 |
| CUST0000000002 | 2022-01-13 12:53:58 | 18 | Male | 60786.11 | master | married | 1 | 22 | one_year | ... | 585 | 0 |
| CUST0000000003 | 2023-09-04 12:53:58 | 38 | Female | 73184.32 | high_school | widowed | 0 | 3 | two_year | ... | 632 | 0 |

Only a small sample is shown due to the size of the dataset.

---

## Raw Features

The original dataset contained the following 32 features:

| Feature | Description |
|---|---|
| customer_id | Unique customer identifier |
| signup_date | Customer registration date |
| age | Customer age |
| gender | Customer gender |
| annual_income | Annual income |
| education | Education level |
| marital_status | Marital status |
| dependents | Number of dependents |
| tenure | Number of months with company |
| contract | Customer contract type |
| payment_method | Payment method |
| paperless_billing | Paperless billing status |
| monthly_charges | Monthly service charges |
| total_charges | Total customer charges |
| num_services | Number of subscribed services |
| has_phone_service | Whether customer has phone service |
| has_internet_service | Whether customer has internet service |
| has_online_security | Online security subscription |
| has_online_backup | Online backup subscription |
| has_device_protection | Device protection subscription |
| has_tech_support | Technical support subscription |
| has_streaming_tv | Streaming TV subscription |
| has_streaming_movies | Streaming movies subscription |
| customer_satisfaction | Customer satisfaction score |
| num_complaints | Number of complaints |
| num_service_calls | Number of service calls |
| late_payments | Number of late payments |
| avg_monthly_gb | Average monthly data usage |
| days_since_last_interaction | Days since last customer interaction |
| credit_score | Customer credit score |
| churn | Target variable (1 = churned, 0 = retained) |

---

# Data Cleaning

The following preprocessing steps were applied:

- Removed `customer_id` as it is a unique identifier and does not provide predictive value.
- Converted `signup_date` into a datetime format.
- Checked missing values across all features.
- Handled missing values using appropriate imputation methods.
- Checked duplicate records.
- Validated feature data types.
- Prepared the dataset for exploratory analysis and machine learning.

---

# Cleaned Dataset

After preprocessing, the final dataset contains:

- 1,000,000 rows
- 31 columns

The cleaned dataset removed the non-predictive `customer_id` column while retaining relevant customer information.

Example structure:

| signup_date | age | gender | annual_income | education | marital_status | dependents | tenure | contract | ... | credit_score | churn |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 2022-12-12 12:53:58 | 43 | Female | 55085.25 | college | married | 1 | 2 | two_year | ... | 680 | 0 |
| 2022-01-13 12:53:58 | 18 | Male | 60786.11 | master | married | 1 | 22 | one_year | ... | 585 | 0 |
| 2023-09-04 12:53:58 | 38 | Female | 73184.32 | high_school | widowed | 0 | 3 | two_year | ... | 632 | 0 |

Only a representative sample is shown.

---

# Final Features Used

The final modelling dataset contains:

| Feature Group | Features |
|---|---|
| Demographics | age, gender, annual_income, education, marital_status, dependents |
| Account | signup_date, tenure, contract, payment_method, paperless_billing |
| Service Usage | monthly_charges, total_charges, num_services, service subscriptions |
| Behaviour | satisfaction, complaints, service calls, late payments, data usage |
| Financial | credit_score |
| Target | churn |

The target variable:

| Value | Meaning |
|---|---|
| 0 | Customer retained |
| 1 | Customer churned |

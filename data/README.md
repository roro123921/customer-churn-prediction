# Dataset

## Overview

This project uses the **Customer Churn Prediction Dataset_1M**, a synthetic telecommunications dataset designed to simulate customer behaviour and churn patterns.

The dataset contains:

- 1,000,000 customer records
- 32 original columns
- 1 binary target variable (`churn`)

The dataset represents customer demographic information, account details, service usage patterns and behavioural indicators.

---

# Raw Dataset

The raw dataset contains customer information before preprocessing.

Example structure:

| customer_id | signup_date | age | gender | annual_income | education | tenure | contract | churn |
|---|---|---|---|---|---|---|---|---|
| CUST0000000001 | 2022-12-12 | 43 | Female | 55085.25 | college | 2 | two_year | 0 |
| CUST0000000002 | 2022-01-13 | 18 | Male | 60786.11 | master | 22 | one_year | 0 |
| CUST0000000003 | 2023-09-04 | 38 | Female | 73184.32 | high_school | 3 | two_year | 0 |

Only a small sample is shown due to the size of the dataset.

---

# Raw Features

## Customer Demographics

| Feature | Description |
|---|---|
| customer_id | Unique customer identifier |
| signup_date | Date customer joined |
| age | Customer age |
| gender | Customer gender |
| annual_income | Annual income |
| education | Education level |
| marital_status | Marital status |
| dependents | Number of dependents |

---

## Account Information

| Feature | Description |
|---|---|
| tenure | Months with company |
| contract | Customer contract type |
| payment_method | Payment method |
| paperless_billing | Paperless billing status |

---

## Service Usage

| Feature | Description |
|---|---|
| monthly_charges | Monthly customer charges |
| total_charges | Total customer charges |
| num_services | Number of subscribed services |
| has_phone_service | Phone service indicator |
| has_internet_service | Internet service indicator |
| has_online_security | Online security subscription |
| has_online_backup | Online backup subscription |
| has_device_protection | Device protection subscription |
| has_tech_support | Technical support subscription |
| has_streaming_tv | Streaming TV subscription |
| has_streaming_movies | Streaming movies subscription |

---

## Customer Behaviour

| Feature | Description |
|---|---|
| customer_satisfaction | Customer satisfaction score |
| num_complaints | Number of complaints |
| num_service_calls | Recent service calls |
| late_payments | Number of late payments |
| avg_monthly_gb | Average monthly data usage |
| days_since_last_interaction | Days since last interaction |
| credit_score | Customer credit score |

---

# Data Cleaning

The raw dataset was processed before modelling.

Cleaning steps included:

- Removed non-predictive identifier (`customer_id`)
- Converted date columns into datetime format
- Checked missing values
- Handled missing values using appropriate methods
- Checked duplicate records
- Validated data types
- Prepared categorical variables for modelling

After preprocessing:

Raw dataset:
- 1,000,000 rows
- 32 columns

Final modelling dataset:
- 1,000,000 rows
- 31 columns

---

# Final Dataset

The cleaned dataset contains customer features ready for exploratory analysis and machine learning.

Example:

| signup_date | age | gender | annual_income | contract | satisfaction | credit_score | churn |
|---|---|---|---|---|---|---|---|
|2022-12-12|43|Female|55085.25|two_year|9|680|0|
|2022-01-13|18|Male|60786.11|one_year|7|585|0|
|2023-09-04|38|Female|73184.32|two_year|6|632|0|

---

# Target Variable

The prediction target is:

`churn`

| Value | Meaning |
|---|---|
|0|Customer retained|
|1|Customer churned|

The model will learn patterns in customer behaviour and account information to predict customers at risk of leaving.

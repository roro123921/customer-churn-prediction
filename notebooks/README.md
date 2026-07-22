# Notebooks
This folder contains the Jupyter notebooks used throughout the customer churn analysis project.

## 1. Data Cleaning
`customer_churn_data_preprocessing.ipynb`

This notebook performs preprocessing on the raw customer churn dataset.

**Steps completed**
- Loaded the raw dataset
- Inspected the dataset structure
- Checked for missing values
- Removed customer ID
- Converted date columns
- Handled missing values
- Checked for duplicate records
- Validated the cleaned dataset
- Exported the cleaned dataset for analysis

## 2. Exploratory Data Analysis
`Customer_Churn_EDA_Notebook_Rohan_Sajeesh.ipynb`

This notebook explores the relationships between customer characteristics and churn through exploratory data analysis and visualisation.

**Analysis includes**
- Overall churn distribution
- Customer demographics
- Contract type and tenure
- Customer satisfaction
- Complaints and service calls
- Payment behaviour
- Service adoption
- Pricing and customer value
- Correlation analysis

The notebook also includes business insights and visualisations that informed the feature engineering stage of the project.

## 3. Feature Engineering and Modelling
`Feature_Engineering_and_Machine_Learning_Modelling.ipynb`

This notebook builds on the EDA findings to prepare the dataset for machine learning and to develop and evaluate classification models predicting customer churn.

**Analysis includes**
- Feature preparation and categorical encoding
- Feature engineering (monthly charge per service)
- Training and comparing five classification models: Logistic Regression, Decision Tree, Random Forest, Gradient Boosting and XGBoost
- Model evaluation under class imbalance (recall, F1-score, ROC-AUC)
- Feature importance and model interpretation
- Business recommendations and limitations

For a concise summary of the full analysis and findings across all three notebooks, see the accompanying report:
- [Customer Churn: End-to-End Data Science Report](../report/Customer_Churn_Final_Report_Rohan_Sajeesh.pdf)

An earlier report, covering only the exploratory analysis stage, is also available for reference:
- [Customer Churn: Exploratory Data Analysis Report](../report/Customer_Churn_EDA_Report_Rohan_Sajeesh.pdf) *(milestone report — superseded by the Final Report above)*

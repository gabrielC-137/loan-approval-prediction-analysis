# Processed Data

This directory contains the cleaned and transformed dataset used for analysis and machine learning models.

---

## File

- **loan_dataset_clean.xlsx**

---

## Data Processing Steps

The dataset underwent the following transformations:

- Imputation of missing values:
  - Categorical variables → mode
  - Numerical variables → median
- Conversion of inconsistent values
- Data type corrections
- Log transformation of skewed variables:
  - ApplicantIncome
  - CoapplicantIncome
  - LoanAmount
- Creation of derived features:
  - Loan_Term_Category (Short, Mid, Long)

---

## Purpose

The processed dataset is used for:

- Exploratory data analysis (EDA)
- Statistical testing (Chi-square)
- Machine learning models:
  - Logistic Regression
  - Random Forest
  - XGBoost

---

## Notes

- This dataset should not be manually modified
- All transformations are documented in the project notebook
- It represents the final analytical dataset used throughout the project

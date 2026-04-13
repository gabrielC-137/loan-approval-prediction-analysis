# Loan Approval Prediction & Risk Analysis

## Overview

This project analyzes a loan application dataset to identify key factors influencing loan approval decisions and to build predictive models for loan eligibility.

The analysis combines exploratory data analysis (EDA), statistical hypothesis testing, feature engineering, and machine learning techniques to understand applicant behavior and improve decision-making processes.

Additionally, an interactive dashboard was developed to translate analytical findings into business insights.

---

## Objectives

- Analyze loan application data to identify patterns and trends  
- Determine the key factors influencing loan approval decisions  
- Perform statistical hypothesis testing to validate relationships between variables  
- Build machine learning models to predict loan approval  
- Evaluate and compare model performance  
- Provide insights to support fair and data-driven credit decisions  

---

## Technologies Used

- Python (Pandas, NumPy, Scikit-learn)
- Machine Learning (Logistic Regression, Random Forest, XGBoost)
- Statistical Analysis (Chi-Square Test)
- Data Preprocessing & Feature Engineering
- Data Visualization
- Power BI

---

## Project Structure

```
loan-approval-prediction-analysis
│
├── README.md
│
├── data
│ ├── raw
│ │ └── loan_dataset.csv
│ └── processed
│ └── loan_dataset_clean.csv
│
├── notebooks
│ └── loan_prediction_code.ipynb
│
└── dashboards
└── dashboard.pbix
```
---

## Data Preparation

The dataset contains 614 loan applications with demographic, financial, and credit-related features.

### Key preprocessing steps:

- Handling missing values:
  - Categorical variables → mode
  - Numerical variables → median  
- Fixing inconsistencies (e.g., "3+" → 3 in Dependents)  
- Log transformation of skewed variables:
  - ApplicantIncome
  - CoapplicantIncome
  - LoanAmount  
- Feature engineering:
  - Creation of **Loan Term Category** (Short, Mid, Long)  

The data was structured into **raw** and **processed** stages to ensure reproducibility and clarity.

---

## Exploratory Data Analysis

EDA was conducted to understand distributions, relationships, and patterns in the dataset.

### Key findings:

- Loan approvals are more frequent than rejections  
- Graduates and married applicants show higher approval rates  
- Semi-urban applicants have the highest approval rates  
- No significant gender bias was observed  
- Strong right-skewed distributions in income and loan amount variables  

---

## Statistical Analysis

Chi-square tests were performed to evaluate relationships between categorical variables and loan approval.

### Key results:

- **Credit History** → Strongest predictor of loan approval  
- **Education Level** → Statistically significant relationship  
- **Property Area** → Significant impact on approval rates  
- **Loan Term Category** → Significant only for medium and long-term loans  

These results confirm that loan approval decisions are strongly influenced by credit-related and demographic factors.

---

## Machine Learning Models

Three classification models were developed and compared:

- Logistic Regression  
- Random Forest  
- XGBoost  

### Evaluation Metrics:

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC  
- Confusion Matrix  

---

## Model Performance Summary

| Model               | Accuracy | ROC-AUC |
|--------------------|---------|--------|
| Logistic Regression| 0.78    | 0.76   |
| Random Forest      | 0.76    | 0.76   |
| XGBoost            | 0.74    | 0.74   |

### Insights:

- Logistic Regression achieved the highest overall accuracy  
- Random Forest provided the most balanced performance  
- XGBoost showed strong recall for approved loans  
- All models confirm the dominant importance of **credit history**  

---

## Key Insights

- Credit history is the most influential factor in loan approval  
- Financial capacity (income and loan amount) plays a significant role  
- Demographic variables have moderate impact  
- Loan approval decisions are largely driven by risk-related features  
- Some variables show weak correlation, suggesting potential for additional features  

---

## Dashboard

An interactive Power BI dashboard was developed to visualize key insights.

<img width="956" height="741" alt="image" src="https://github.com/user-attachments/assets/9d8c6442-931e-470e-837f-e3f83f653154" />



### Features:

- Loan approval distribution  
- Approval rates by education, marital status, and location  
- Credit history impact analysis  
- Loan term category insights  
- Interactive exploration of approval patterns  

---

## Conclusion

This project demonstrates how combining statistical analysis with machine learning can provide meaningful insights into loan approval processes.

The results highlight the importance of credit history and financial indicators in determining loan eligibility, while also emphasizing the need for balanced and fair decision-making systems.


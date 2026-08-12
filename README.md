# Loan Status Prediction

## Project Overview

This project uses Machine Learning to predict whether a loan application will be **Approved** or **Rejected** based on applicant demographics, income, credit history, and loan characteristics.

The project covers data preprocessing, exploratory data analysis, feature engineering, model development, and performance comparison.

## Dataset

The dataset contains **3,192 loan applications** with the following information:

- Gender
- Married
- Dependents
- Education
- Employment Status
- Applicant Income
- Coapplicant Income
- Loan Amount
- Loan Term
- Credit History
- Property Area
- Age
- Loan Status

## Project Workflow

### 1. Data Cleaning

- Checked missing values
- Handled missing categorical values using the mode
- Handled missing numerical values using the median
- Checked for duplicate records

### 2. Exploratory Data Analysis

Analyzed loan approval patterns across:

- Gender
- Marital Status
- Education
- Employment Status
- Income
- Loan Amount
- Loan Term
- Credit History
- Age
- Property Area
- Dependents

### 3. Feature Engineering

Created additional financial features:

- Total Income
- Monthly Income
- Loan-to-Income Ratio
- Loan Amount per Term

Categorical variables were encoded, resulting in **18 features** for model development.

### 4. Model Development

The dataset was split into training and testing sets using an 80/20 split.

The following models were trained and evaluated:

- Logistic Regression
- Random Forest
- Gradient Boosting

## Model Performance

| Model | Accuracy |
|---|---:|
| Logistic Regression | **98.44%** |
| Gradient Boosting | **98.12%** |
| Random Forest | **97.81%** |

**Logistic Regression achieved the highest accuracy of 98.44%.**

## Key Insights

- Analyzed **3,192 loan applications** to evaluate demographics, income, credit history, and loan characteristics.
- Performed data preprocessing, EDA, and feature engineering to prepare **18 features** for model development.
- Compared Logistic Regression, Random Forest, and Gradient Boosting models.
- **Credit History** was identified as the most influential factor affecting overall loan approval predictions.

## Project Results

### Loan Status Distribution
![Feature Importance](screenshots/feature-importance.png)

### Feature Importance

![Loan Status Distribution](screenshots/loan-status-distribution.png)

### Model Performance

![Model Performance](screenshots/model-performance.png)

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Repository Structure

```text
loan-status-prediction/
│
├── Loan_Status_Prediction.ipynb
├── train.csv
├── requirements.txt
├── README.md
│
└── screenshots/
    ├── loan-status-distribution.png
    ├── feature-importance.png
    └── model-performance.png

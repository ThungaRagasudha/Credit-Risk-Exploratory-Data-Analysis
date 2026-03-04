# **Credit Risk Analysis – Exploratory Data Analysis (EDA)**
## Project Overview
This project performs Exploratory Data Analysis (EDA) on a real-world Credit Risk Dataset (32,000+ records) to identify patterns and risk factors that influence loan default.

Loan default is a major challenge for banks, NBFCs, and fintech companies. By analyzing borrower demographics, financial attributes, and loan characteristics, this project aims to uncover key indicators of credit risk that can support better lending decisions.

The analysis focuses on understanding borrower behavior and identifying relationships between financial variables that contribute to default risk.

## Project Objectives

- Analyze borrower demographic and financial attributes
- Identify patterns that influence loan default
- Understand relationships between income, loan amount, interest rate, credit grade, and loan purpose
- Detect risk indicators associated with high default probability
- Generate data-driven insights useful for credit risk assessment

## Dataset Information
- **Dataset**: Credit Risk Dataset
- **Source**: Kaggle
- **Records**: ~32,000+
- **Features**: 12 (Numerical + Categorical)
- **Target Variable**:
    `loan_status`
    - **0 → Non-Default**
    - **1 → Default**

## Key Features in Dataset
### Demographic Features
- `person_age` – Age of borrower
- `person_home_ownership` – Housing ownership status
- `person_emp_length` – Employment length
### Financial Features
- `person_income` – Annual income
- `loan_amnt` – Loan amount
- `loan_int_rate` – Interest rate
- `loan_percent_income` – Loan as a percentage of income
- `loan_grade` – Credit grade
- `cb_person_cred_hist_length` – Credit history length
### Behavioral Feature
- `loan_intent` – Purpose of loan

## Data Cleaning & Preprocessing
The dataset was prepared before analysis through the following steps:
- Inspected dataset structure and data types
- Removed duplicate records
- Handled missing values in:
  - loan_int_rate
  - person_emp_length
- Applied Median Imputation for numerical missing values
- Checked class imbalance in loan_status
- Identified skewness and outliers using histograms and boxplots

#  Exploratory Data Analysis

## Univariate Analysis
Purpose: Understand the distribution of individual variables.

### Techniques Used
- Histogram
- Box Plot
- Count Plot
  
### Key Observations
- Income distribution is right-skewed
- Most borrowers belong to the working-age group
- Dataset shows class imbalance (non-defaults dominate)
 
## Bivariate Analysis
Purpose: Explore relationships between variables and default behavior.

### Techniques Used
- Scatter Plots (Income vs Loan Amount)
- Bar Plots (Default Rate by Loan Intent)
- Count Plots (Loan Grade vs Default)
- Grouped aggregations using Pandas

### Key Findings
- Higher income borrowers tend to take larger loans
- Medical and debt consolidation loans have higher default rates
- Loan purpose significantly impacts repayment behavior
- Lower loan grades are associated with higher default ratios

## Multivariate Analysis
Purpose: Identify complex interactions between multiple features.

### Techniques Used
- Correlation Heatmap
- Pair Plot
- Feature interaction analysis

### Key Insights
- Loan-to-income ratio strongly influences default risk
- Higher interest rates correlate with higher defaults
- Longer credit history reduces default probability
- Income alone is not sufficient to predict repayment

## Business Insights
- Borrowers with high loan burden (loan % of income) are more likely to default
- Interest rate and credit grade are strong indicators of credit risk
- Credit history length improves repayment reliability
- Loan purpose plays a critical role in risk profiling
- Effective credit risk assessment requires multi-variable analysis

## Tools & Technologies
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

## Conclusion

This project demonstrates how Exploratory Data Analysis (EDA) can uncover meaningful insights from financial datasets.

The analysis highlights important risk factors such as loan burden, interest rate, credit grade, and credit history, which play a key role in predicting loan default.

These insights can support financial institutions in improving credit risk assessment, lending decisions, and borrower risk profiling.

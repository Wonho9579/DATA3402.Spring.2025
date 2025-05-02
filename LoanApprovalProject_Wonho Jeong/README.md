# Loan Approval Classification Project

## Overview
This project aims to predict whether a loan application will be approved using four key financial features. The analysis is based on a synthetic dataset and follows the official class guidelines for the final tabular Kaggle project in DATA3402.

## Dataset
The dataset was generated using a synthetic loan approval generator, similar in structure to the Kaggle dataset:  
["Financial Risk for Loan Approval"](https://www.kaggle.com/datasets/lorenzozoppelletto/financial-risk-for-loan-approval)

We selected four features for simplicity and focus:
- `CreditScore` (numerical)
- `AnnualIncome` (numerical)
- `EmploymentStatus` (categorical, one-hot encoded)
- `TotalDebtToIncomeRatio` (numerical)

Target:
- `LoanApproved` (binary: 0 = Not Approved, 1 = Approved)

## Project Steps (Following Class Guidelines)
1. **Define Project**: Binary classification (Loan approval).
2. **Initial Look**: Loaded 20,000 rows, confirmed no missing values.
3. **Feature Summary**: Each feature was evaluated for type, value range, and outliers.
4. **Visualization**: Histograms and bar charts showed clear class differences.
5. **Data Preparation**:
   - One-hot encoded `EmploymentStatus`
   - Standard scaled numerical features
6. **Model Training**: Logistic Regression using train/test split.
7. **Model Evaluation**:
   - Accuracy: **86.8%**
   - F1-score for approved class: **0.70**
   - Confusion matrix included
8. **Submission File**: Model applied to test set and predictions saved to `loan_approval_submission.csv`.

## Final Performance Summary
- Accuracy: **0.86825**
- Precision (Approved): 0.77
- Recall (Approved): 0.63
- F1-score (Approved): 0.70

## Files Included
- `Loan_Project.ipynb`: Full analysis notebook
- `loan_approval_submission.csv`: Model predictions
- `README.md`: Project overview (this file)

## Author
Wonho Jeong  
DATA 3402 - Spring 2025


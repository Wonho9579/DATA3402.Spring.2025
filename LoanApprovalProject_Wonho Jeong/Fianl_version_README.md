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
4. **Visualization**:
   - Compared feature distributions between classes using histograms (numerical) and bar charts (categorical).
   - Identified class imbalance in the target variable.
5. **Data Preparation**:
   - One-hot encoded `EmploymentStatus`
   - Standard scaled numerical features using `StandardScaler`
   - Visualized each numerical feature before and after scaling using side-by-side KDE plots (subplot format)
6. **Model Training**:
   - Applied `LogisticRegression` using `train_test_split` (80/20) with stratified sampling.
   - Trained the model using selected and preprocessed features.
7. **Model Evaluation**:
   - Accuracy: **86.8%**
   - Precision, Recall, and F1-score evaluated using `classification_report`
   - Confusion matrix clearly showed correct vs incorrect predictions
8. **Submission File**:
   - Predictions on the test set were saved to `loan_approval_submission.csv` in proper Kaggle format

## Final Performance Summary
- Accuracy: **0.86825**
- Precision (Approved): 0.77
- Recall (Approved): 0.63
- F1-score (Approved): 0.70

## Files Included
- `Loan_Project_Wonho_Jeong.ipynb`: Full analysis notebook
- `loan_approval_submission.csv`: Model predictions on the test set
- `README.md`: Project overview and step-by-step summary

## Author
Wonho Jeong  
DATA 3402 - Spring 2025


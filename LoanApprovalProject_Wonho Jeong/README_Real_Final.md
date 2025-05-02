
# Loan Approval Classification Project

## 📌 Overview
This project predicts whether a loan application will be approved using four key features:
- CreditScore
- AnnualIncome
- EmploymentStatus
- TotalDebtToIncomeRatio

The problem is binary classification with the target variable `LoanApproved` (0 = not approved, 1 = approved).  
The dataset is synthetic and contains 20,000 rows with no missing values.

---

## 📊 Step 1: Initial Data Exploration

![Step 2 Data Preview](./project_images/step2_data_preview.PNG)

---

## 📋 Step 2: Feature Summary

![Feature Summary Table](./project_images/feature_summary_table.PNG)

---

## 📈 Step 3: Feature Visualization by Loan Approval

**Credit Score Distribution**

![CreditScore](./project_images/credit_score_by_approval.png)

**Annual Income Distribution**

![AnnualIncome](./project_images/annual_income_by_approval.png)

**Debt-to-Income Ratio Distribution**

![DTI](./project_images/dti_by_approval.png)

**Employment Status Bar Chart**

![Employment](./project_images/employment_bar.png)

---

## ⚙️ Step 4: Feature Preparation and Scaling

**Scaled: Credit Score**

![Scaled CreditScore](./project_images/scaled_credit_score.png)

**Scaled: Annual Income**

![Scaled Income](./project_images/scaled_annual_income.png)

**Scaled: Debt-to-Income Ratio**

![Scaled DTI](./project_images/scaled_dti.png)

---

## ⚠️ Step 5: Class Imbalance Check

- LoanApproved = 0 (Not Approved): 76.1%
- LoanApproved = 1 (Approved): 23.9%

---

## 🤖 Step 6: Model Training and Evaluation

![Classification Report](./project_images/classification_report.PNG)

- Model: Logistic Regression
- Accuracy: 86.8%
- F1-score (Approved): 0.70
- Confusion Matrix showed 606 correct approvals

---

## 📤 Step 7: Kaggle-style Submission File

![Submission Preview](./project_images/submission_preview.PNG)

The index values may look shuffled because the test set was randomly split,  
but each prediction correctly maps to its original test sample.

---

## ✅ Conclusion

This project helped me go through the entire machine learning pipeline:  
from defining the problem, exploring and visualizing the data, to building and evaluating a model.

A key insight was that **CreditScore**, **EmploymentStatus**, and **Debt-to-Income Ratio**  
were the strongest features affecting loan approval.

It was a valuable experience that made me more confident in solving real-world problems with data.

NAME:SUSREE PATRO
SEC:D
LAB_SEC:D1
CLASS ROLL NO:39
LAB_ROLL_NO:20

📘 Loan Default Prediction — ML Pipeline

This project builds a machine learning system to predict whether a borrower will pay back a loan or default, using data from FinSecure, a peer-to-peer lending company. The goal is to help the loan approval team make faster, data-driven, and fair decisions.

🔍 Project Overview

The target variable loan_paid_back indicates whether a loan was repaid (1) or defaulted (0).
This project includes:

Data cleaning & preprocessing

Outlier removal

Feature engineering

Model training (Logistic Regression & Random Forest)

ROC–AUC performance comparison

Fairness analysis across borrower subgroups

📂 Dataset Summary

The dataset includes:

Financial features: income, debt-to-income ratio, credit score

Loan features: amount, interest rate, purpose

Demographics: gender, marital status, education

Assigned grade/subgrade

Target: loan_paid_back

🧹 Preprocessing Steps

Missing values handled using median (numeric) & mode (categorical)

Outliers removed using IQR method (before/after boxplots included)

One-hot encoding for categorical variables

Standard scaling for numeric features

Train–test split (80/20 with stratification)

🤖 Models Used

1. Logistic Regression
Baseline linear model for comparison.

2. Random Forest Classifier
Captures non-linear patterns and usually delivers higher AUC.

Both models output the probability of loan repayment.

📈 Evaluation
ROC–AUC Curves

AUC is calculated and plotted for both models.
This measures how well the model distinguishes paid vs. defaulted loans.

Subgroup AUC (Fairness Check)

Performance is compared across:

Different education levels

Top and bottom loan purposes

This ensures the model does not unfairly penalize certain groups.

🧪 Visualizations

The script generates:

Target distribution plot

Boxplots before/after outlier removal

ROC–AUC curves

Subgroup AUC tables

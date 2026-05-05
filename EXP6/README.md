# EXP 6 - Credit Risk Assessment (Credit Scoring)

## Overview
This experiment builds a **credit scoring / credit risk assessment model** to evaluate the creditworthiness of loan applicants using historical financial and behavioral data. Multiple classification models are trained and compared to analyze performance.

## Problem Statement
Build a model that predicts an applicant’s **Credit Risk** category using past financial attributes and repayment behavior, and perform a comparative analysis of:
- Logistic Regression
- Random Forest
- XGBoost (XGBClassifier)

## Dataset
Dataset file:
- `credit_risk_assessment_500_samples.csv`

### Columns (Features)
- `Applicant_ID` - Unique applicant identifier  
- `Age` - Applicant age  
- `Annual_Income` - Annual income of applicant  
- `Employment_Years` - Years of employment experience  
- `Credit_Score` - Credit score value  
- `Loan_Amount` - Requested loan amount  
- `Loan_Term_Months` - Loan duration (months)  
- `Existing_Loans_Count` - Number of existing loans  
- `Debt_to_Income_Ratio` - Debt-to-income ratio  
- `Late_Payments_Last_2Yrs` - Late payments count in last 2 years  

### Target Column
- `Credit_Risk` - Risk category (`Low`, `Medium`, `High`)

## Workflow / Pipeline
1. Import required libraries
2. Load the dataset
3. Data understanding (shape, null checks, basic stats)
4. Preprocessing
   - Encode categorical target labels using **LabelEncoder**
5. Feature/target split
6. Train-test split
7. Train and compare models:
   - Logistic Regression
   - Random Forest Classifier
   - XGBoost Classifier
8. Prediction on test set
9. Evaluation and comparison using:
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Confusion Matrix
   - Classification Report
   - ROC-AUC and ROC Curve (where applicable)

## Libraries Used
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
  - `train_test_split`, `LabelEncoder`
  - Models: `LogisticRegression`, `RandomForestClassifier`
  - Metrics: `accuracy_score`, `precision_score`, `recall_score`, `f1_score`,
    `confusion_matrix`, `classification_report`, `roc_auc_score`, `roc_curve`
- `xgboost`
  - `XGBClassifier`

## Notebook
Run the experiment using:
- `Experiment6.ipynb`

## How to Run
1. Open `Experiment6.ipynb` in Jupyter Notebook / Google Colab.
2. Ensure `credit_risk_assessment_500_samples.csv` is accessible (or update the dataset path in the notebook).
3. Run all cells in order.
4. Observe evaluation metrics and ROC/Confusion Matrix outputs for model comparison.

## Expected Outcome
A trained credit risk classifier that categorizes applicants into **Low / Medium / High** risk, and a comparison of model performance to determine the best algorithm for the dataset.

## Conclusion
This experiment demonstrates how machine learning can be applied in the finance domain for **credit risk scoring**, and how different classification algorithms perform on the same credit dataset.

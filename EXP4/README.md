# EXP 4 - Customer Churn Prediction

## Overview
This experiment focuses on predicting customer churn in a subscription-based business using classification and data analysis techniques. The goal is to identify customers who are likely to leave the service based on their demographic, billing, and engagement information.

## Problem Statement
Develop a model to predict customer churn using customer-related features such as age, tenure, subscription type, monthly charges, payment method, support tickets, and contract type.

## Dataset Description
The dataset used in this experiment is:

- `customer_churn_dataset.csv`

### Features
- `CustomerID` - Unique customer identifier
- `Gender` - Customer gender
- `Age` - Customer age
- `Tenure_Months` - Number of months the customer has stayed
- `SubscriptionType` - Type of subscription (`Basic`, `Standard`, `Premium`)
- `MonthlyCharges` - Monthly billing amount
- `TotalCharges` - Total amount charged
- `PaymentMethod` - Mode of payment used
- `SupportTickets` - Number of support tickets raised
- `ContractType` - Type of contract (`Month-to-Month`, `One Year`, `Two Year`)
- `Churn` - Target variable indicating whether the customer left (`1`) or stayed (`0`)

## Workflow
1. Load the dataset
2. Understand the data structure
3. Perform preprocessing and encoding
4. Split features and target variable
5. Split the dataset into training and testing sets
6. Train a regression or classification model
7. Make predictions
8. Evaluate the model using:
   - Accuracy
   - Precision
   - Recall
9. Perform graphical analysis

## Libraries Used
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

## Model Used
A machine learning classification model is used to predict whether a customer will churn.

## How to Run
1. Open the notebook `Experiment_4.ipynb`
2. Ensure the dataset file is available in the correct path
3. Run all notebook cells sequentially
4. Review the predictions, metrics, and visualizations

## Expected Outcome
The model should help identify customers at risk of churn, enabling businesses to take proactive retention actions.

## Conclusion
This experiment demonstrates the use of machine learning for customer churn prediction and exploratory data analysis.

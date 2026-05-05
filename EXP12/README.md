# EXP 12 - Melbourne Housing Price Prediction (Ensemble Learning)

## Overview
This experiment focuses on predicting **house prices** using the **Melbourne Housing dataset**. The key objective is to build a robust regression pipeline with proper preprocessing for mixed (numerical + categorical) features, and to apply **ensemble learning** techniques to improve prediction performance.

## Problem Statement
Develop a machine learning model to predict housing prices using the Melbourne housing dataset, and analyze model performance using appropriate regression evaluation metrics. Emphasis is placed on using **ensemble methods** and comparing results against baseline approaches.

## Files in this Folder
- `Experiment12.ipynb` — Notebook implementation (data loading, preprocessing, model training, evaluation)
- `dataset_Melbourne_housing_FULL_exp_12.csv` — Dataset used for the experiment
- `Experiment12_Report.pdf` — Experiment 12 report
- `Exp-11-12.pdf` — Document containing Experiment 11 & 12 content
- `README.md` — This file

## Dataset
File: `dataset_Melbourne_housing_FULL_exp_12.csv`

The dataset contains Melbourne housing records with a mix of:
- **Numerical features** (e.g., rooms, distance, bedroom count, bathroom count, etc.)
- **Categorical features** (e.g., suburb, type, method, seller, region, council area, etc.)

### Target Variable
- House **Price** (the value the model learns to predict)

## Workflow / Pipeline
1. Import required libraries
2. Load the Melbourne housing dataset
3. Exploratory Data Analysis (EDA)
   - Check dataset shape, columns, missing values
   - Understand distributions and correlations (as needed)
4. Data preprocessing
   - Handle missing values (imputation or removal depending on columns)
   - Encode categorical variables (e.g., one-hot encoding)
   - Feature scaling for numerical variables (if required by the model)
5. Split into training and testing sets
6. Train regression models (baseline + ensemble)
7. Generate predictions on test set
8. Evaluate using regression metrics such as:
   - MAE (Mean Absolute Error)
   - MSE / RMSE (Mean Squared Error / Root Mean Squared Error)
   - R² Score
9. Compare model performance and summarize results

## Models Used (Typical Comparative Setup)
This experiment is structured for ensemble-based regression. Common models used for comparison include:
- Linear Regression (baseline)
- Decision Tree Regressor
- Random Forest Regressor (ensemble)
- Gradient Boosting / XGBoost (ensemble, if used in the notebook)

*(Refer to `Experiment12.ipynb` for the exact set of models implemented.)*

## Libraries Commonly Used
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
  - preprocessing + encoding utilities
  - regression models and ensemble models
  - metrics for regression evaluation

## How to Run
1. Open `Experiment12.ipynb` in Jupyter Notebook / Google Colab.
2. Ensure `dataset_Melbourne_housing_FULL_exp_12.csv` is available in the `EXP12` folder (or update the dataset path in the notebook).
3. Run all cells sequentially to reproduce preprocessing, training, and evaluation results.
4. Review metrics and comparisons to identify the best-performing model.

## Expected Outcome
- A complete regression pipeline capable of predicting Melbourne house prices.
- Performance comparison showing the benefits of ensemble learning over simpler baseline models.

## Conclusion
This experiment demonstrates how real-world housing datasets require careful preprocessing and how ensemble regression methods can significantly improve price prediction performance.

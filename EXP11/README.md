# EXP 11 - Diabetes Prediction using Bagging Ensemble (with Model Comparison)

## Overview
This experiment predicts whether a person has **diabetes** (`Outcome`) based on medical diagnostic features such as glucose level, blood pressure, BMI, age, etc. The main focus is implementing the **Bagging Ensemble technique** and performing a **comparative analysis** with other classification models.

## Problem Statement
Predict whether a person has diabetes using patient health features by applying:
- **Bagging Ensemble (BaggingClassifier)**
and compare performance with baseline models such as:
- Decision Tree
- Logistic Regression
- Random Forest

## Files in this Folder
- `Experiment11.ipynb` — Complete implementation (EDA → preprocessing → training → evaluation)
- `dataset_diabetes_exp_11.csv` — Dataset used for training/testing
- `Experiment11_Report.pdf` — Report for Experiment 11
- `Exp-11-12.pdf` — Document for Experiments 11 & 12
- `README.md` — This file

## Dataset
File: `dataset_diabetes_exp_11.csv`  
Shape (as shown in notebook): **768 rows × 9 columns**

### Features (Input)
- `Pregnancies`
- `Glucose`
- `BloodPressure`
- `SkinThickness`
- `Insulin`
- `BMI`
- `DiabetesPedigreeFunction`
- `Age`

### Target (Output)
- `Outcome`
  - `0` = No Diabetes
  - `1` = Diabetes

## Workflow / Pipeline
1. Import required libraries
2. Load dataset
3. Exploratory Data Analysis (EDA)
   - Dataset info, statistics
   - Class distribution (bar chart + pie chart)
   - Feature distributions (histograms)
   - Boxplots
   - Correlation heatmap and correlations with `Outcome`
4. Data preprocessing
   - **Invalid zero handling**:
     - Columns treated: `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, `BMI`
     - Zeros replaced with **median** of non-zero values
   - **Outlier handling**:
     - IQR-based outlier detection
     - Outliers capped using lower/upper IQR bounds
5. Feature/Target split
6. Train-test split + cross-validation (Stratified K-Fold used in notebook)
7. Model training & comparison
   - Bagging ensemble and baseline models
8. Model evaluation
   - Accuracy, Precision, Recall, F1-score
   - Confusion matrix
   - Classification report
   - ROC Curve and ROC-AUC (where applicable)

## Models Used
- `DecisionTreeClassifier` (base estimator)
- `BaggingClassifier`
- `LogisticRegression`
- `RandomForestClassifier`

## Libraries Used
- `numpy`, `pandas`
- `matplotlib`, `seaborn`
- `scikit-learn`
  - Preprocessing: `StandardScaler`, `Pipeline`
  - Model selection: `train_test_split`, `cross_val_score`, `StratifiedKFold`
  - Models: `DecisionTreeClassifier`, `BaggingClassifier`, `LogisticRegression`, `RandomForestClassifier`
  - Metrics: `accuracy_score`, `precision_score`, `recall_score`, `f1_score`,
    `confusion_matrix`, `classification_report`, `roc_curve`, `roc_auc_score`, `auc`

## How to Run
1. Open `Experiment11.ipynb` in Jupyter Notebook / Google Colab.
2. Ensure `dataset_diabetes_exp_11.csv` is available in the same folder (or update the dataset path in the notebook).
3. Run cells sequentially to reproduce:
   - EDA visualizations
   - preprocessing steps (zero imputation + outlier capping)
   - model training and evaluation results

## Expected Outcome
- A working diabetes prediction pipeline.
- Clear performance comparison showing how **Bagging Ensemble** performs relative to other classifiers.

## Conclusion
This experiment demonstrates how ensemble learning (bagging) can improve stability and performance in medical classification tasks, along with proper preprocessing (invalid values + outlier treatment) and detailed evaluation.

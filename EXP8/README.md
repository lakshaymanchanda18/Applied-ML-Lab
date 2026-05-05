# EXP 8 - Multiclass Classification: Student Performance Level Analysis

## Overview
This experiment implements **multiclass classification models** to analyze and predict **students’ performance levels** based on academic and behavioral features such as study hours, attendance, assignment score, internal marks, participation, internet access, and previous grade.

A comparative analysis is performed across multiple ML models to evaluate which algorithm gives the best results.

## Problem Statement
Implement multiclass classification models for **Student Performance Level** prediction and perform comparative analysis using:
- Random Forest
- Decision Tree
- Multinomial Logistic Regression
- XGBoost
- K-Nearest Neighbors (KNN)

## Dataset
Dataset file:
- `multiclass_classification_dataset_500_samples.csv`

### Columns (Features)
- `Study_Hours` - Hours studied by the student
- `Attendance_Percentage` - Attendance percentage
- `Assignment_Score` - Assignment performance score
- `Internal_Marks` - Internal assessment marks
- `Participation` - Participation level (`Low`, `Medium`, `High`)
- `Internet_Access` - Internet availability (`Yes` / `No`)
- `Previous_Grade` - Previous grade (e.g., `A`, `B`, `C`)

### Target Column
- `Performance_Level` - Multiclass label (e.g., `0`, `1`, `2` depending on encoding in the dataset)

## Methodology / Workflow
1. Import required libraries
2. Load dataset and inspect structure
3. Data preprocessing
   - Encode categorical features using **LabelEncoder**
   - Scale numerical features using **StandardScaler**
4. Split dataset into training and testing sets
5. Train and compare models:
   - Decision Tree Classifier
   - Random Forest Classifier
   - Logistic Regression (Multinomial)
   - K-Nearest Neighbors
   - XGBoost Classifier
6. Generate predictions on test set
7. Evaluate and compare models using:
   - Accuracy
   - Precision (macro/weighted as applicable)
   - Recall (macro/weighted as applicable)
   - F1-score (macro/weighted as applicable)
   - Confusion Matrix
   - Classification Report

## Libraries Used
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
  - Preprocessing: `LabelEncoder`, `StandardScaler`
  - Models: `DecisionTreeClassifier`, `RandomForestClassifier`, `LogisticRegression`, `KNeighborsClassifier`
  - Utilities: `train_test_split`
  - Metrics: `accuracy_score`, `precision_score`, `recall_score`, `f1_score`,
    `confusion_matrix`, `classification_report`
- `xgboost`
  - `XGBClassifier`

## Notebook
Run the experiment using:
- `Experiment8.ipynb`

## How to Run
1. Open `Experiment8.ipynb` in Jupyter Notebook / Google Colab.
2. Ensure `multiclass_classification_dataset_500_samples.csv` is accessible (or update the dataset path inside the notebook).
3. Run all cells sequentially.
4. Compare model results using printed metrics and confusion matrices.

## Expected Outcome
A multiclass classification pipeline that predicts student performance levels and provides a comparative performance summary across multiple models.

## Conclusion
This experiment demonstrates how multiclass ML models can be applied to educational datasets for performance analysis, and shows how different algorithms perform on the same classification task.

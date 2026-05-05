# EXP 9 - Physiological Signal Classification (Normal vs Abnormal)

## Overview
This experiment implements machine learning classification models to distinguish between **normal** and **abnormal physiological (ECG/heartbeat) signals** using extracted signal features. A comparative analysis is performed across multiple ML classifiers to evaluate performance.

The experiment is based on the **Heartbeat (ECG) dataset** commonly used for arrhythmia / abnormal heartbeat detection.

## Problem Statement
Implement a classification model to distinguish between **normal** and **abnormal** physiological signals using extracted signal features, and perform comparative analysis across different ML models.

**Dataset link:** https://www.kaggle.com/datasets/shayanfazeli/heartbeat

## Dataset
The notebook loads the following CSV files (from the Kaggle dataset):

### MIT-BIH Arrhythmia Dataset (Multi-class ECG beats)
- `mitbih_train.csv`
- `mitbih_test.csv`

### PTB Diagnostic ECG Database (Binary: normal vs abnormal)
- `ptbdb_normal.csv`
- `ptbdb_abnormal.csv`

> Note: These CSVs contain extracted/processed heartbeat signal samples as numeric feature vectors.  
> In MIT-BIH files, the **last column** is the label, and the remaining columns represent features.

## Models Used (Comparative Analysis)
The following classifiers are trained and compared:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

## Workflow / Pipeline
1. Import required libraries
2. Load datasets (MIT-BIH + PTBDB)
3. Preprocessing
   - Separate features (`X`) and labels (`y`)
   - Standardize features using **StandardScaler**
4. Train-test split (where applicable)
5. Train multiple classification models
6. Predict on test data
7. Evaluate models using:
   - Accuracy
   - Confusion Matrix
   - Classification Report (Precision, Recall, F1-score)

## Libraries Used
- `pandas`, `numpy`
- `scikit-learn`
  - Preprocessing: `StandardScaler`
  - Models:
    - `LogisticRegression`
    - `KNeighborsClassifier`
    - `DecisionTreeClassifier`
    - `RandomForestClassifier`
    - `SVC`
  - Metrics:
    - `accuracy_score`
    - `confusion_matrix`
    - `classification_report`

## Notebook
Run the experiment using:
- `Experiment9.ipynb`

## How to Run
1. Download the dataset from Kaggle: https://www.kaggle.com/datasets/shayanfazeli/heartbeat
2. Place the following files in the `EXP9/` directory (or update paths in the notebook):
   - `mitbih_train.csv`, `mitbih_test.csv`
   - `ptbdb_normal.csv`, `ptbdb_abnormal.csv`
3. Open `Experiment9.ipynb` in Jupyter Notebook / Google Colab.
4. Run all cells sequentially.
5. Compare model performance using accuracy, confusion matrices, and classification reports.

## Expected Outcome
A trained classifier that can distinguish between normal and abnormal heartbeat patterns, along with a comparison showing which ML model performs best on the dataset.

## Conclusion
This experiment demonstrates how machine learning models can be applied to healthcare signal datasets for **abnormality detection**, and how classifier choice impacts performance in physiological signal classification tasks.

# EXP 7 - Anomaly Detection (Outlier / Fraud Detection)

## Overview
This experiment implements an **anomaly detection system** to identify **outliers** in a dataset (commonly used in fraud detection, intrusion detection, and fault detection). Multiple anomaly detection algorithms are trained and compared to analyze which method detects anomalies more effectively.

## Problem Statement
Implement an anomaly detection system for detecting outliers in data and perform a comparative analysis of:
- Isolation Forest
- Local Outlier Factor (LOF)
- One-Class SVM

## Dataset
Dataset file:
- `anomaly_detection_dataset_500_samples.csv`

### Columns
- `Feature_1` - Numeric feature
- `Feature_2` - Numeric feature
- `Anomaly_Label` - Ground truth label:
  - `0` = Normal (inlier)
  - `1` = Anomaly (outlier)

## Methodology / Workflow
1. Import required libraries
2. Load the dataset
3. Data understanding (distribution, imbalance check, visualization)
4. Preprocessing
   - Feature scaling using **StandardScaler**
   - Encode labels if required
5. Train-test split (for evaluation and comparison)
6. Train and compare anomaly detection models:
   - **Isolation Forest**
   - **Local Outlier Factor (LOF)**
   - **One-Class SVM**
7. Prediction (inlier vs outlier)
8. Evaluation and comparison using:
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Confusion Matrix
   - Classification Report

> Note: Many anomaly detection models output `-1` for anomaly and `1` for normal. These predictions are mapped to match the dataset labels for evaluation.

## Libraries Used
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
  - Preprocessing: `StandardScaler`, `LabelEncoder`
  - Models: `IsolationForest`, `LocalOutlierFactor`, `OneClassSVM`
  - Utilities: `train_test_split`
  - Metrics: `accuracy_score`, `precision_score`, `recall_score`, `f1_score`,
    `confusion_matrix`, `classification_report`

## Notebook
Run the experiment using:
- `Experiment7.ipynb`

## How to Run
1. Open `Experiment7.ipynb` in Jupyter Notebook / Google Colab.
2. Ensure `anomaly_detection_dataset_500_samples.csv` is accessible (or update the dataset path inside the notebook).
3. Run all cells sequentially.
4. Compare results of Isolation Forest, LOF, and One-Class SVM using metrics and confusion matrices.

## Expected Outcome
A working anomaly detection pipeline that identifies outliers and provides a performance comparison across different anomaly detection algorithms.

## Conclusion
This experiment demonstrates anomaly detection using multiple ML approaches and highlights how different models behave when detecting rare abnormal data points.

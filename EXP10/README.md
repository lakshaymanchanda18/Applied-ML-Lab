# EXP 10 - Iris Flower Classification

## Overview
This experiment implements a **multiclass classification model** using the classic **Iris dataset** to predict the species of iris flowers based on their sepal and petal measurements. The dataset is loaded directly from `sklearn.datasets`.

## Problem Statement
**Iris Flower Classification:** Build a classification model that predicts the species of iris flowers using the Iris dataset.

**Dataset Source:** `sklearn.datasets.load_iris()`

## Files in this Folder
- `Experiment10.ipynb` — Notebook implementation (data loading, EDA, training, evaluation, testing on new input)
- `Experiment10_Report.pdf` — Experiment report
- `Exp_9_10.docx` — Document for experiments (9 & 10)
- `README.md` — This file

## Dataset Details
The Iris dataset contains **150 samples** with **4 features** and **3 classes**.

### Features (Input)
- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

### Target Classes (Output)
- `setosa`
- `versicolor`
- `virginica`

## Workflow / Pipeline
1. Load Iris dataset using `load_iris()`
2. Understand dataset structure (feature names, target names, shapes)
3. Convert dataset into a Pandas DataFrame for easier analysis
4. Perform basic EDA
   - Class distribution using `value_counts()`
5. Visualization
   - Pairplot using Seaborn (`sns.pairplot`) to visualize separation between classes
6. Train-test split (`test_size=0.2`, `random_state=42`)
7. Model training
   - K-Nearest Neighbors (KNN) classifier with `n_neighbors=3`
8. Model prediction on test set
9. Evaluation
   - Accuracy score
   - Confusion matrix
   - Classification report (precision, recall, f1-score)
10. Test the model using a new flower sample input

## Model Used
- **K-Nearest Neighbors (KNN) Classifier**
  - `KNeighborsClassifier(n_neighbors=3)`

## Libraries Used
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
  - `load_iris`
  - `train_test_split`
  - `KNeighborsClassifier`
  - `accuracy_score`, `confusion_matrix`, `classification_report`

## How to Run
1. Open `Experiment10.ipynb` in Jupyter Notebook / Google Colab.
2. Run all cells sequentially (no external dataset download required).
3. Review outputs:
   - dataset details
   - visualizations (pairplot)
   - evaluation metrics and confusion matrix
4. (Optional) Modify the sample input to test predictions on new measurements.

## Expected Outcome
- A trained KNN classifier that predicts iris species.
- Model evaluation metrics (accuracy, confusion matrix, classification report).
- Ability to classify a new sample flower using the trained model.

## Conclusion
This experiment demonstrates a complete ML workflow for a simple multiclass classification problem using the Iris dataset, including dataset exploration, visualization, model training, evaluation, and prediction on new samples.

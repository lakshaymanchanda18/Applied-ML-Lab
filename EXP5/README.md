# EXP 5 - Spam Email Detection (Text Classification)

## Overview
This experiment builds a **spam email detection system** using **text classification** techniques. Emails are converted into numerical features using TF-IDF, and multiple machine learning classifiers are trained and compared to determine which performs best for spam detection.

## Problem Statement
Build a spam email filter using text classification algorithms and perform a comparative analysis of multiple models:
- Naïve Bayes
- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest

## Dataset
Dataset file (used in the notebook):
- `spam_email.csv`

The dataset contains email text (message/content) along with a label indicating whether the email is **Spam** or **Not Spam (Ham)**.

## Methodology / Workflow
1. **Import libraries**
2. **Load dataset**
3. **Text preprocessing & feature extraction**
   - Convert text to feature vectors using **TF-IDF Vectorizer**
4. **Train-test split**
5. **Model training** (multiple classifiers)
6. **Prediction**
7. **Evaluation & comparison**
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Confusion Matrix
   - ROC-AUC (where applicable)
   - Classification Report
   - ROC Curve

## Libraries Used
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
  - `TfidfVectorizer`
  - Models:
    - `MultinomialNB`
    - `LogisticRegression`
    - `SVC`
    - `DecisionTreeClassifier`
    - `RandomForestClassifier`
  - Metrics:
    - `accuracy_score`, `precision_score`, `recall_score`, `f1_score`
    - `confusion_matrix`, `classification_report`
    - `roc_auc_score`, `roc_curve`

## Notebook
Run the experiment using:
- `Experiment5.ipynb`

## How to Run
1. Open `Experiment5.ipynb` in Jupyter Notebook / Google Colab.
2. Ensure `spam_email.csv` is accessible (either in the same folder or update the dataset path inside the notebook).
3. Run all cells sequentially.
4. Compare model performance using the printed metrics and plots.

## Expected Outcome
A trained spam classifier that can classify emails as **Spam** or **Ham**, along with a comparison of multiple algorithms to identify the best-performing approach for the dataset.

## Conclusion
This experiment demonstrates the complete workflow of **text feature extraction + supervised classification**, and highlights how different ML algorithms perform on spam detection tasks.

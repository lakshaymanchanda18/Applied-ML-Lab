# Applied Machine Learning Lab 🚀
## A Comprehensive Collection of ML Experiments & Real-World Applications

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square&logo=jupyter)](https://jupyter.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-green?style=flat-square&logo=scikit-learn)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)]()

**Professional-grade ML implementations covering supervised learning, classification, anomaly detection, and ensemble methods.**

[Quick Start](#quick-start) • [Experiments](#experiments) • [Technologies](#technologies) • [Contributing](#contributing)

</div>

---

## 📋 Overview

This repository is a **comprehensive applied machine learning laboratory** featuring **12 progressive experiments** that span fundamental ML concepts to advanced ensemble techniques. Each experiment is designed for practical understanding and includes:

- ✅ Complete Jupyter notebooks with detailed implementations
- ✅ Real-world datasets with preprocessing workflows  
- ✅ Multiple model comparisons and performance analysis
- ✅ Professional documentation and comprehensive reports
- ✅ Production-ready code patterns and best practices

**Target Audience:** ML practitioners, data scientists, students, and professionals seeking to strengthen their applied ML skills through hands-on implementations.

---

## 🎯 Quick Start

### Prerequisites
```bash
Python 3.8+
Jupyter Notebook / JupyterLab / Google Colab
```

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/lakshaymanchanda18/Applied-ML-Lab.git
cd Applied-ML-Lab
```

2. **Create a virtual environment (recommended)**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install numpy pandas scikit-learn matplotlib seaborn xgboost jupyter
```

4. **Launch Jupyter**
```bash
jupyter notebook
```

### Running an Experiment
Navigate to any experiment folder (e.g., `EXP1/`) and open the Jupyter notebook:
```bash
cd EXP1
jupyter notebook Experiment_1.ipynb
```

---

## 📊 Experiments Overview

### **Experiment 1: Introduction to Applied Machine Learning** 🔧
**Path:** `EXP1/Experiment_1.ipynb`

| Aspect | Details |
|--------|---------|
| **Objective** | Foundational ML pipeline workflow |
| **Focus** | Data loading, preprocessing, model training, evaluation |
| **Models** | Basic ML model(s) from scikit-learn |
| **Key Concepts** | Train-test split, feature engineering, evaluation metrics |
| **Dataset** | Custom structured data (`data.csv`) |
| **Outputs** | Model predictions, performance metrics |

**Key Learnings:**
- Setting up a complete ML pipeline
- Data preprocessing best practices
- Model evaluation and interpretation

---

### **Experiment 2: Housing Price Prediction (Regression)** 🏠
**Path:** `EXP2/Experiment_2.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Predict residential property prices |
| **Dataset** | 120 housing records with mixed features |
| **Target** | House price (continuous) |
| **Models** | Regression algorithms |
| **Key Features** | Location, area, rooms, amenities, age, furnish status |
| **Evaluation** | MSE, R² Score, MAE |

**Models Implemented:**
- Linear Regression
- Multiple Regression with feature engineering
- Model comparison and hyperparameter tuning

**Real-World Application:** Real estate valuation, investment analysis, property market prediction

---

### **Experiment 3: Stock Price Forecasting (Time Series Regression)** 📈
**Path:** `EXP3/Experiment_3.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Predict stock prices from historical data |
| **Dataset** | Stock market data with OHLC features |
| **Target** | Stock price (continuous) |
| **Models** | Time-series regression models |
| **Features** | Open, High, Low, Close, Volume |
| **Evaluation** | MSE, R², prediction accuracy |

**Models Implemented:**
- Linear Regression for time series
- Feature engineering from OHLC data
- Performance evaluation on financial data

**Real-World Application:** Financial forecasting, algorithmic trading, investment decision support

---

### **Experiment 4: Customer Churn Prediction (Binary Classification)** 👥
**Path:** `EXP4/Experiment_4.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Identify customers likely to leave |
| **Dataset** | 500+ customer subscription data |
| **Target** | Churn (binary: Yes/No) |
| **Models** | Classification algorithms |
| **Key Features** | Demographics, tenure, charges, contract type, support tickets |
| **Evaluation** | Accuracy, Precision, Recall, F1-score, ROC-AUC |

**Models Implemented:**
- Logistic Regression
- Decision Tree Classifier
- Ensemble methods comparison

**Real-World Application:** Customer retention strategy, lifetime value prediction, risk assessment

---

### **Experiment 5: Spam Email Detection (Text Classification)** 📧
**Path:** `EXP5/Experiment5.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Classify emails as spam or ham |
| **Dataset** | Spam email dataset with text content |
| **Target** | Email type (binary: Spam/Ham) |
| **Models** | 5 different classifiers |
| **Feature Extraction** | TF-IDF Vectorization |
| **Evaluation** | Accuracy, Precision, Recall, F1-score, ROC-AUC, Classification Report |

**Models Implemented:**
- ✅ Multinomial Naive Bayes
- ✅ Logistic Regression
- ✅ Support Vector Machine (SVM)
- ✅ Decision Tree
- ✅ Random Forest

**Comparative Analysis:** Performance comparison across all 5 models with visualizations

**Real-World Application:** Email filtering systems, spam detection, content moderation, security

---

### **Experiment 6: Credit Risk Assessment (Multiclass Classification)** 💳
**Path:** `EXP6/Experiment6.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Assess loan applicant credit risk |
| **Dataset** | 500 applicant credit records |
| **Target** | Credit Risk (multiclass: Low/Medium/High) |
| **Models** | 3 advanced classifiers |
| **Key Features** | Age, income, employment, credit score, loan amount, debt ratio, late payments |
| **Evaluation** | Accuracy, Precision, Recall, F1-score, Confusion Matrix, ROC-AUC |

**Models Implemented:**
- ✅ Logistic Regression
- ✅ Random Forest Classifier
- ✅ XGBoost Classifier

**Comparative Analysis:** Model performance comparison with ROC curves and confusion matrices

**Real-World Application:** Loan underwriting, credit scoring, financial risk management, lending decisions

---

### **Experiment 7: Anomaly Detection (Outlier/Fraud Detection)** 🚨
**Path:** `EXP7/Experiment7.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Detect anomalies/outliers in data |
| **Dataset** | 500-sample anomaly detection dataset |
| **Target** | Anomaly Label (binary: Normal/Anomaly) |
| **Models** | 3 unsupervised anomaly detectors |
| **Feature Scaling** | StandardScaler normalization |
| **Evaluation** | Accuracy, Precision, Recall, F1-score, Confusion Matrix |

**Models Implemented:**
- ✅ Isolation Forest
- ✅ Local Outlier Factor (LOF)
- ✅ One-Class SVM

**Comparative Analysis:** Performance across all 3 anomaly detection approaches

**Real-World Application:** Fraud detection, intrusion detection, system fault identification, data quality monitoring

---

### **Experiment 8: Multiclass Classification - Student Performance Analysis** 🎓
**Path:** `EXP8/Experiment8.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Predict student performance levels |
| **Dataset** | 500 student records with academic metrics |
| **Target** | Performance Level (multiclass) |
| **Models** | 5 diverse classifiers |
| **Features** | Study hours, attendance, assignment scores, internal marks, participation, internet access, previous grade |
| **Evaluation** | Accuracy, Precision, Recall, F1-score, Confusion Matrix, Classification Report |

**Models Implemented:**
- ✅ Random Forest Classifier
- ✅ Decision Tree Classifier
- ✅ Multinomial Logistic Regression
- ✅ K-Nearest Neighbors (KNN)
- ✅ XGBoost Classifier

**Comparative Analysis:** Comprehensive model comparison with detailed performance metrics

**Real-World Application:** Educational assessment, student success prediction, personalized learning paths, institutional planning

---

### **Experiment 9: Physiological Signal Classification (ECG Heartbeat Analysis)** 🫀
**Path:** `EXP9/Experiment9.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Classify normal vs. abnormal ECG signals |
| **Dataset** | Kaggle Heartbeat dataset (MIT-BIH + PTBDB) |
| **Target** | Signal Type (binary: Normal/Abnormal) |
| **Models** | 5 medical-grade classifiers |
| **Signal Features** | Extracted heartbeat characteristics (188 features) |
| **Evaluation** | Accuracy, Confusion Matrix, Classification Report, Precision, Recall, F1-score |

**Models Implemented:**
- ✅ Logistic Regression
- ✅ K-Nearest Neighbors (KNN)
- ✅ Decision Tree
- ✅ Random Forest
- ✅ Support Vector Machine (SVM)

**Dataset Source:** [Kaggle Heartbeat Dataset](https://www.kaggle.com/datasets/shayanfazeli/heartbeat)

**Real-World Application:** Cardiac health monitoring, arrhythmia detection, ECG analysis automation, telemedicine

---

### **Experiment 10: Iris Flower Classification (Multiclass Classification)** 🌸
**Path:** `EXP10/Experiment10.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Classify iris flower species |
| **Dataset** | Classic Iris dataset (150 samples, 3 species) |
| **Target** | Iris Species (multiclass: setosa/versicolor/virginica) |
| **Models** | K-Nearest Neighbors with optimal parameters |
| **Features** | Sepal length, sepal width, petal length, petal width |
| **Evaluation** | Accuracy, Confusion Matrix, Classification Report, Pairplot visualization |

**Models Implemented:**
- ✅ K-Nearest Neighbors (KNN, n_neighbors=3)

**Visualizations:** Seaborn pairplot for feature relationships and class separation

**Real-World Application:** Classic ML benchmark, botanical species identification, introduction to multiclass classification

---

### **Experiment 11: Diabetes Prediction (Ensemble Learning - Bagging)** 🏥
**Path:** `EXP11/Experiment11.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Predict diabetes risk from medical metrics |
| **Dataset** | 768 patient records with medical diagnostics |
| **Target** | Diabetes Status (binary: Yes/No) |
| **Models** | Bagging ensemble + 3 baseline models |
| **Key Features** | Pregnancies, glucose, blood pressure, skin thickness, insulin, BMI, age, diabetes pedigree |
| **Evaluation** | Accuracy, Precision, Recall, F1-score, ROC-AUC, Cross-validation scores |

**Preprocessing Techniques:**
- Invalid value handling (zero imputation using median)
- Outlier detection and capping (IQR method)
- Feature scaling and standardization

**Models Implemented:**
- ✅ Decision Tree Classifier (base)
- ✅ Bagging Classifier (ensemble)
- ✅ Logistic Regression (baseline)
- ✅ Random Forest Classifier (comparison)

**Advanced Features:**
- Stratified K-Fold cross-validation
- ROC Curve and AUC analysis
- Detailed preprocessing pipeline

**Real-World Application:** Healthcare diagnosis support, disease risk prediction, medical data analysis, patient screening

---

### **Experiment 12: Melbourne Housing Price Prediction (Ensemble Regression)** 🏘️
**Path:** `EXP12/Experiment12.ipynb`

| Aspect | Details |
|--------|---------|
| **Problem** | Predict Melbourne house prices |
| **Dataset** | 13,580+ property records with mixed feature types |
| **Target** | House Price (continuous regression) |
| **Models** | Ensemble regression methods with baselines |
| **Feature Types** | Numerical (rooms, distance, etc.) + Categorical (suburb, type, region, etc.) |
| **Evaluation** | MAE, MSE, RMSE, R² Score |

**Preprocessing Challenges:**
- Mixed numerical and categorical features
- Missing value imputation strategies
- Categorical encoding (one-hot encoding)
- Feature scaling for numerical features
- Large dataset optimization

**Models Implemented:**
- ✅ Linear Regression (baseline)
- ✅ Decision Tree Regressor
- ✅ Random Forest Regressor (ensemble)
- ✅ Gradient Boosting / XGBoost (advanced ensemble)

**Real-World Application:** Real estate pricing, market analytics, investment valuation, property listing recommendation

---

## 🛠 Technologies & Libraries

### Core ML & Data Processing
```
scikit-learn      1.0+      (ML models, preprocessing, metrics)
pandas            1.3+      (Data manipulation & analysis)
numpy             1.20+     (Numerical computing)
```

### Visualization & Analysis
```
matplotlib        3.4+      (Static plotting & visualization)
seaborn          0.11+      (Statistical data visualization)
```

### Advanced Algorithms
```
xgboost          1.5+       (Gradient boosting framework)
```

### Development Environment
```
jupyter          1.0+       (Interactive notebooks)
python           3.8+       (Programming language)
```

---

## 📁 Repository Structure

```
Applied-ML-Lab/
├── EXP1/                           # Introduction to ML
│   ├── Experiment_1.ipynb
│   ├── Pandas_Practice_Questions.pdf
│   ├── data.csv
│   └── README.md
│
├── EXP2/                           # Housing Price Prediction (Regression)
│   ├── Experiment_2.ipynb
│   ├── Exp2_Housing_Price_Dataset_120_Records.csv
│   ├── Experiment2_Report.pdf
│   ├── Pipeline_Steps-Regression.pdf
│   ├── Regression_Questions.pdf
│   └── README.md
│
├── EXP3/                           # Stock Price Forecasting
│   ├── Experiment_3.ipynb
│   ├── stock_price_with_price_column.csv
│   ├── Experiment3_Report.pdf
│   ├── Regression_Questions.pdf
│   └── README.md
│
├── EXP4/                           # Customer Churn Prediction
│   ├── Experiment_4.ipynb
│   ├── customer_churn_dataset.csv
│   ├── Experiment4_Report.pdf
│   ├── Regression_Questions.pdf
│   └── README.md
│
├── EXP5/                           # Spam Email Detection (Text Classification)
│   ├── Experiment5.ipynb
│   ├── spam_email.csv
│   ├── Experiment5_Report.pdf
│   ├── Exp 5_6_7_8 (Question).pdf
│   └── README.md
│
├── EXP6/                           # Credit Risk Assessment
│   ├── Experiment6.ipynb
│   ├── credit_risk_assessment_500_samples.csv
│   ├── Experiment6_Report.pdf
│   ├── Exp 5_6_7_8 (Question).pdf
│   └── README.md
│
├── EXP7/                           # Anomaly Detection
│   ├── Experiment7.ipynb
│   ├── anomaly_detection_dataset_500_samples.csv
│   ├── Experiment7_Report.pdf
│   ├── Exp 5_6_7_8 (Question).pdf
│   └── README.md
│
├── EXP8/                           # Multiclass Classification - Student Performance
│   ├── Experiment8.ipynb
│   ├── multiclass_classification_dataset_500_samples.csv
│   ├── Experiment8_Report.pdf
│   ├── Exp 5_6_7_8 (Question).pdf
│   └── README.md
│
├── EXP9/                           # ECG Signal Classification
│   ├── Experiment9.ipynb
│   ├── Experiment9_Report.pdf
│   ├── Exp_9_10.docx
│   └── README.md
│
├── EXP10/                          # Iris Flower Classification
│   ├── Experiment10.ipynb
│   ├── Experiment10_Report.pdf
│   ├── Exp_9_10.docx
│   └── README.md
│
├── EXP11/                          # Diabetes Prediction (Bagging Ensemble)
│   ├── Experiment11.ipynb
│   ├── dataset_diabetes_exp_11.csv
│   ├── Experiment11_Report.pdf
│   ├── Exp-11-12.pdf
│   └── README.md
│
├── EXP12/                          # Melbourne Housing Price Prediction
│   ├── Experiment12.ipynb
│   ├── dataset_Melbourne_housing_FULL_exp_12.csv
│   ├── Experiment12_Report.pdf
│   ├── Exp-11-12.pdf
│   └── README.md
│
├── AML_LabReportFile.pdf           # Comprehensive lab report
├── README.md                       # This file
└── requirements.txt                # Python dependencies
```

---

## 🎓 Learning Outcomes

By working through this repository, you will master:

### **Foundational Concepts**
- ✅ Complete ML pipeline architecture
- ✅ Data preprocessing & cleaning workflows
- ✅ Feature engineering techniques
- ✅ Train-test split strategies
- ✅ Model evaluation and metric interpretation

### **Supervised Learning**
- ✅ Regression (linear, multiple, time-series)
- ✅ Binary classification (churn, fraud, spam)
- ✅ Multiclass classification (risk levels, species, performance)
- ✅ Performance metrics (accuracy, precision, recall, F1, ROC-AUC, MAE, MSE, R²)

### **Advanced Techniques**
- ✅ Ensemble methods (Bagging, Random Forest, XGBoost)
- ✅ Anomaly detection algorithms
- ✅ Text classification & NLP preprocessing
- ✅ Medical signal analysis
- ✅ Cross-validation strategies
- ✅ Hyperparameter tuning
- ✅ Model comparison and selection

### **Real-World Applications**
- ✅ Real estate valuation
- ✅ Financial forecasting
- ✅ Customer retention strategy
- ✅ Healthcare diagnosis support
- ✅ Fraud detection systems
- ✅ Educational assessment

### **Professional Skills**
- ✅ Jupyter notebook best practices
- ✅ Code documentation & comments
- ✅ Data visualization & storytelling
- ✅ Report writing and presentation
- ✅ Reproducible research practices

---

## 📈 Experiment Progression Map

```
EXP1: Foundation
   ↓
EXP2-3: Regression Tasks
   ↓
EXP4-8: Classification Tasks
   ↓
EXP9-10: Specialized Classification
   ↓
EXP11-12: Ensemble & Advanced Methods
```

**Recommended Learning Path:**
1. Start with **EXP1** for foundational concepts
2. Move to **EXP2-3** for regression understanding
3. Progress through **EXP4-8** for classification techniques
4. Explore **EXP9-10** for specialized domains
5. Master **EXP11-12** for ensemble and production methods

---

## 🔬 Model Comparison Summary

| Experiment | Primary Models | Key Metrics | Best For |
|------------|----------------|-----------|----------|
| EXP1 | Basic ML | Baseline metrics | Foundation |
| EXP2 | Linear Regression | MSE, R² | Housing valuation |
| EXP3 | Time-Series Regression | RMSE, MAE | Financial forecasting |
| EXP4 | Classification models | Accuracy, F1 | Customer retention |
| EXP5 | 5 Text Classifiers | Precision, Recall, ROC-AUC | Spam filtering |
| EXP6 | 3 Credit Classifiers | Accuracy, F1, ROC-AUC | Risk assessment |
| EXP7 | 3 Anomaly Detectors | Accuracy, F1 | Fraud detection |
| EXP8 | 5 Multiclass Models | Macro F1, Weighted F1 | Student assessment |
| EXP9 | 5 Signal Classifiers | Accuracy, Precision | Medical diagnosis |
| EXP10 | KNN | Accuracy, Confusion Matrix | Species classification |
| EXP11 | Bagging Ensemble | Accuracy, ROC-AUC | Disease prediction |
| EXP12 | Ensemble Regression | RMSE, R² | Property valuation |

---

## 💡 Key Features & Highlights

✨ **Complete Implementations**
- Every experiment includes data loading, preprocessing, model training, and evaluation
- Real-world datasets with actual complexity (missing values, outliers, imbalance)

🎯 **Model Comparisons**
- Multiple algorithms tested on the same dataset
- Performance comparison with visualizations
- Clear best-practice recommendations

📊 **Visualization-Rich**
- Confusion matrices, ROC curves, feature importance plots
- Pairplots, correlation heatmaps, distribution analysis
- Professional-grade visualizations using matplotlib & seaborn

📚 **Well-Documented**
- Detailed README files for each experiment
- Inline code comments explaining logic
- Comprehensive reports in PDF format

🔧 **Production-Ready Code**
- Error handling and input validation
- Modular function design
- Reproducible results with random seeds

---

## 📖 How to Use This Repository

### For Learning
1. Read the experiment's README in its folder
2. Open the Jupyter notebook
3. Run cells sequentially and understand each step
4. Modify code to experiment with variations
5. Review the experiment report for deeper insights

### For Reference
- Use as a template for your own ML projects
- Copy code patterns for specific tasks
- Adapt models for your datasets
- Reference best practices and workflows

### For Benchmarking
- Compare your model implementations
- Validate metric calculations
- Use as baseline for performance comparison

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Report Issues** - Found a bug? Open an issue with details
2. **Suggest Improvements** - Propose enhancements or new experiments
3. **Code Contributions** - Submit pull requests with improvements
4. **Documentation** - Help improve documentation and comments
5. **Experiments** - Suggest new ML applications and datasets

### Contribution Guidelines
- Follow PEP 8 Python style guide
- Add meaningful comments to code
- Include experiment documentation
- Test your code thoroughly
- Create descriptive commit messages

---

## 📝 Citation & References

If you use this repository in your work, please cite:

```bibtex
@repository{appliedmllib2024,
  title = {Applied Machine Learning Lab},
  author = {Lakshay Manchanda},
  year = {2024},
  url = {https://github.com/lakshaymanchanda18/Applied-ML-Lab}
}
```

### Datasets Used
- Kaggle Heartbeat Dataset: https://www.kaggle.com/datasets/shayanfazeli/heartbeat
- Iris Dataset: Standard sklearn dataset
- Melbourne Housing Dataset: Real estate data
- Custom datasets provided for credit, churn, and spam classification

---

## 📄 License

This project is licensed under the **MIT License** - see the LICENSE file for details.

---

## 🔗 Resources & Links

### Documentation
- [scikit-learn Documentation](https://scikit-learn.org/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [XGBoost Documentation](https://xgboost.readthedocs.io/)
- [Jupyter Documentation](https://jupyter.org/)

### Learning Resources
- [Kaggle Datasets](https://www.kaggle.com/datasets)
- [Machine Learning Mastery](https://machinelearningmastery.com/)
- [Papers with Code](https://paperswithcode.com/)

### Tools
- [Google Colab](https://colab.research.google.com/) - Free GPU notebooks
- [Jupyter Lab](https://jupyterlab.readthedocs.io/) - Enhanced notebook environment
- [VS Code Jupyter Extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

---

## 📞 Contact & Support

- **Author:** Lakshay Manchanda
- **GitHub:** [@lakshaymanchanda18](https://github.com/lakshaymanchanda18)
- **Repository:** [Applied-ML-Lab](https://github.com/lakshaymanchanda18/Applied-ML-Lab)

For questions or suggestions, please open an issue in the repository.

---

## 🎯 Future Enhancements

Planned additions:
- [ ] Deep Learning experiments (Neural Networks, CNN, RNN)
- [ ] Time Series forecasting with ARIMA/Prophet
- [ ] Reinforcement Learning basics
- [ ] Natural Language Processing (NLP) projects
- [ ] Computer Vision applications
- [ ] Model deployment tutorials
- [ ] Advanced hyperparameter optimization
- [ ] AutoML implementations
- [ ] Feature engineering best practices
- [ ] MLOps and production pipelines

---

<div align="center">

### ⭐ If you find this helpful, please consider giving it a star! ⭐

Made with ❤️ for the ML community

</div>

---

**Last Updated:** May 2026 | **Status:** Active & Maintained

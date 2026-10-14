# Customer Churn Prediction Pipeline

## Author

Wayne Franz

---

# Project Overview

This project demonstrates an end-to-end machine learning workflow for predicting customer churn using Python, Scikit-Learn, Jupyter Notebook, and Git.

Customer churn occurs when a customer stops using a company's products or services. By predicting churn, businesses can proactively identify customers at risk of leaving and implement retention strategies before churn occurs.

The project follows professional machine learning engineering practices and includes data exploration, preprocessing, model development, model comparison, and deployment-ready pipeline creation.

---

# Business Problem

Customer acquisition is typically more expensive than customer retention.

The objective of this project is to develop a machine learning model capable of predicting whether a customer is likely to churn based on demographic information, account details, billing information, and service usage patterns.

Accurate churn prediction can help organizations:

- Improve customer retention
- Reduce revenue loss
- Increase customer lifetime value
- Improve marketing effectiveness
- Support data-driven business decisions

---

# Dataset

## Dataset Source

IBM Telco Customer Churn Dataset

## Machine Learning Task

**Binary Classification**

Predict whether a customer is likely to churn.

### Target Variable

**Churn**

- Yes = Customer Churned
- No = Customer Retained

### Features

The dataset includes:

- Customer demographics
- Senior citizen status
- Partner status
- Dependents
- Account tenure
- Internet service type
- Contract type
- Payment method
- Monthly charges
- Total charges
- Service subscriptions
- Technical support usage

---

# Project Structure

```text
ml-portfolio-project/

├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_project_setup.ipynb
│   ├── 02_data_understanding.ipynb
│   ├── 03_eda.ipynb
│   ├── 04_feature_engineering.ipynb
│   ├── 05_model_baseline.ipynb
│   ├── 06_model_comparison.ipynb
│   └── 07_final_pipeline.ipynb
│
├── models/
│   └── trained_models/
│
├── reports/
│   ├── figures/
│   └── presentations/
│
├── src/
│   ├── config.py
│   ├── evaluation.py
│   └── __init__.py
│
├── README.md
├── LICENSE
├── requirements.txt
└── .gitignore
```

---

# Technology Stack

## Programming Language

- Python

## Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Joblib

## Development Tools

- VS Code
- Jupyter Notebook
- Git
- GitHub

---

# Project Workflow

## Phase 1: Data Understanding

- Load dataset
- Explore dataset structure
- Examine data types
- Identify missing values
- Investigate target variable

## Phase 2: Exploratory Data Analysis (EDA)

- Distribution analysis
- Churn analysis
- Feature relationship analysis
- Data visualization
- Business insight generation

## Phase 3: Feature Engineering

- Data cleaning
- TotalCharges correction
- Removal of identifier fields
- Train-test split
- Feature preprocessing pipelines
- One-Hot Encoding
- Feature scaling

## Phase 4: Baseline Modelling

- Logistic Regression baseline model
- Performance evaluation

## Phase 5: Model Comparison

Models evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting

## Phase 6: Final Pipeline

- Final model selection
- Production pipeline creation
- Model serialization
- Deployment preparation

---

# Exploratory Data Analysis Findings

The strongest predictors of customer churn were:

- Customer tenure
- Contract type
- Internet service type
- Monthly charges

Key observations included:

- Month-to-month customers churn more frequently
- Customers with shorter tenure are more likely to churn
- Fiber Optic customers exhibit higher churn rates
- Customers with higher monthly charges are more likely to churn

---

# Model Performance

## Models Evaluated

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---------|---------|---------|---------|---------|---------|
| Logistic Regression | 0.8038 | 0.6485 | 0.5722 | 0.6080 | 0.8359 |
| Gradient Boosting | 0.7967 | 0.6429 | 0.5294 | 0.5806 | 0.8386 |
| Random Forest | 0.7875 | 0.6307 | 0.4840 | 0.5477 | 0.8137 |
| Decision Tree | 0.7306 | 0.4934 | 0.4973 | 0.4953 | 0.6565 |

---

# Final Model

## Selected Model

**Logistic Regression**

Although Gradient Boosting achieved a slightly higher ROC-AUC score, Logistic Regression was selected because it delivered:

- Highest Accuracy
- Highest Precision
- Highest Recall
- Highest F1 Score
- Excellent interpretability
- Simpler deployment

### Final Performance

| Metric | Score |
|----------|----------|
| Accuracy | 0.8038 |
| Precision | 0.6485 |
| Recall | 0.5722 |
| F1 Score | 0.6080 |
| ROC-AUC | 0.8359 |

---

# Project Deliverables

This project includes:

- Professional GitHub repository
- Well-documented Jupyter notebooks
- Data visualizations
- Feature engineering pipeline
- Model comparison framework
- Production-ready machine learning pipeline
- Saved deployment artifact

---

# Key Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Machine Learning
- Model Evaluation
- Pipeline Construction
- Git Version Control
- Technical Documentation
- Deployment Preparation

---

# Future Improvements

Potential future enhancements include:

- Hyperparameter tuning using GridSearchCV
- Cross-validation analysis
- Feature importance investigation
- SHAP explainability
- XGBoost implementation
- Streamlit deployment
- Cloud deployment using Azure Machine Learning

---

# License

This project is licensed under the MIT License. See the LICENSE file for details.
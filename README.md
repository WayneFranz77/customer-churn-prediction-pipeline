Customer Churn Prediction Pipeline
Author
Wayne Franz

Project Overview
This portfolio project demonstrates an end-to-end machine learning workflow for predicting customer churn.

Customer churn occurs when a customer stops using a company's products or services. Predicting churn allows businesses to proactively identify at-risk customers and implement retention strategies before customers leave.

The project will be developed using professional machine learning engineering practices and will result in a reproducible, production-ready machine learning pipeline.

Business Problem
Customer acquisition is often more expensive than customer retention.

The objective of this project is to build a machine learning model capable of predicting whether a customer is likely to churn based on demographic, account, and service usage information.

By identifying customers with a high probability of churning, a business can:

Improve customer retention
Reduce revenue loss
Increase customer lifetime value
Improve marketing efficiency
Support data-driven decision making
Project Goals
The goals of this project are to:

Build a complete machine learning workflow
Perform exploratory data analysis (EDA)
Clean and preprocess raw data
Engineer meaningful features
Compare multiple machine learning models
Tune model hyperparameters
Build a reusable machine learning pipeline
Evaluate model performance
Save and document the final model
Showcase machine learning engineering skills in a professional portfolio
Dataset
Target Variable
Customer Churn

0 = Customer Retained
1 = Customer Churned
Potential Features
Customer information may include:

Customer demographics
Contract type
Service subscriptions
Internet service type
Payment method
Monthly charges
Total charges
Account tenure
Customer support usage
Project Structure
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
├── src/
│   ├── config.py
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   ├── modeling.py
│   ├── evaluation.py
│   └── utils.py
│
├── models/
│   └── trained_models/
│
├── reports/
│   ├── figures/
│   └── presentation/
│
├── README.md
├── requirements.txt
└── .gitignore
Workflow
Phase 1: Data Understanding
Load dataset
Review structure
Examine data types
Identify target variable
Identify missing values
Phase 2: Exploratory Data Analysis
Descriptive statistics
Distribution analysis
Correlation analysis
Churn analysis
Visualization development
Phase 3: Data Preparation
Missing value treatment
Categorical encoding
Feature scaling
Data splitting
Phase 4: Feature Engineering
Create derived features
Evaluate feature importance
Remove redundant variables
Phase 5: Model Development
Models to evaluate may include:

Logistic Regression
Decision Tree
Random Forest
Gradient Boosting
XGBoost (optional)
Phase 6: Hyperparameter Tuning
Grid Search
Cross Validation
Pipeline optimization
Phase 7: Final Pipeline
Build end-to-end pipeline
Save trained model
Export reproducible workflow
Evaluation Metrics
Model performance will be evaluated using:

Accuracy
Precision
Recall
F1 Score
ROC-AUC
Because customer churn datasets are frequently imbalanced, special attention will be given to Recall, F1 Score, and ROC-AUC.

Expected Deliverables
Professional GitHub repository
Jupyter notebooks
Reusable Python modules
Trained machine learning model
Final machine learning pipeline
Visualizations and reports
Project documentation
Success Criteria
A successful project will:

Produce reproducible results
Follow machine learning engineering best practices
Achieve strong predictive performance
Demonstrate end-to-end pipeline development
Be suitable for inclusion in a professional portfolio
Dataset Selection
Dataset
IBM Telco Customer Churn Dataset

Description
The dataset contains customer demographic information, account information, subscribed services, and customer churn status.

The objective is to predict whether a customer will leave the company's service.

Target Variable
Churn

Yes = Customer churned
No = Customer retained
Expected Features
Gender
Senior Citizen Status
Partner
Dependents
Tenure
Phone Service
Internet Service
Contract Type
Payment Method
Monthly Charges
Total Charges
Why This Dataset?
This dataset is well-suited for machine learning engineering because it contains:

Numerical and categorical variables
Missing values to handle
Opportunities for feature engineering
A business-focused prediction task
A binary classification target
Machine Learning Task
Binary Classification

Predict whether a customer is likely to churn based on customer characteristics and service usage.
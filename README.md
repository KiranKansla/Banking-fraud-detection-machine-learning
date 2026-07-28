# 🏦 Banking Fraud Detection using Python & Machine Learning

![Project Cover](Images/cover.png)

An end-to-end Machine Learning project that predicts fraudulent banking transactions using Python and Scikit-learn. The project covers the complete data science workflow, including Exploratory Data Analysis (EDA), Feature Engineering, Data Preprocessing, Machine Learning Model Development, Model Evaluation, and Business Recommendations.

## Project Overview

Financial institutions process millions of digital transactions every day, making fraud detection a critical business challenge. Traditional rule-based systems often struggle to detect evolving fraud patterns while minimizing false positives.

This project develops a Machine Learning solution capable of identifying fraudulent transactions using behavioral, transactional, and risk-related features. Multiple classification models were trained and evaluated to determine the most effective fraud detection approach.

## Business Problem

The primary objective of this project is to identify fraudulent banking transactions before financial losses occur.

The project answers key business questions:

- Which customer behaviors are most associated with fraud?
- Which variables contribute most to fraud prediction?
- Which Machine Learning model performs best?
- How accurately can fraudulent transactions be identified?
- What business actions can reduce fraud risk?

## Dataset Overview

The dataset simulates modern digital banking transactions with realistic customer behavior and fraud scenarios.

It includes:

- Transaction Amount
- Login Attempts
- Device Risk Score
- Transfer Frequency
- AI Anomaly Score
- Account Age
- Geographic Distance
- Transaction Velocity
- Authentication Method
- Payment Channel
- Suspicious IP Flag
- International Transaction Flag
- Fraud Label

### Dataset Summary

| Metric | Value |
|---------|------:|
| Total Transactions | **10,000** |
| Fraudulent Transactions | **1,251** |
| Fraud Rate | **12.51%** |
| Total Transaction Amount | **$124.13 Million** |
| Fraudulent Transaction Amount | **Approximately $16 Million** |

## Project Workflow

### 1. Data Cleaning

- Missing value validation
- Duplicate checking
- Data type verification
- Outlier assessment

### 2. Exploratory Data Analysis

Analyzed:

- Fraud distribution
- Transaction amount distribution
- Anomaly score distribution
- Transaction patterns
- Correlation analysis
- Fraud by payment channel
- Fraud by authentication method

### 3. Feature Engineering

Created features for Machine Learning by:

- Encoding categorical variables
- Scaling numerical variables
- Selecting predictive features
- Preparing training and testing datasets

### 4. Machine Learning Models

The following classification algorithms were trained and evaluated:

- Logistic Regression
- Decision Tree
- Random Forest

## Model Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|--------|----------:|----------:|--------:|----------:|---------:|
| Logistic Regression | 95.35% | 84.00% | 77.60% | 80.70% | **97.9%** |
| Decision Tree | 94.45% | 78.14% | 77.20% | 77.67% | - |
| Random Forest | **95.25%** | **82.70%** | **78.40%** | **80.49%** | **97.5%** |

## Key Findings

- Fraud represented **12.51%** of all transactions.
- Approximately **$16 Million** in transaction value was identified as fraudulent.
- **Anomaly Score** was the strongest predictor of fraud.
- The correlation between Fraud Label and Anomaly Score was approximately **0.67**.
- Mobile banking transactions contributed the highest fraudulent transaction value.
- Random Forest achieved the best balance between Accuracy, Precision, Recall, and F1 Score.
- Logistic Regression achieved the highest ROC-AUC score, demonstrating excellent classification capability.

## Visualizations

The project includes:

- Fraud Distribution
- Transaction Amount Distribution
- Boxplots
- Correlation Heatmap
- Anomaly Score Distribution
- Feature Importance
- Confusion Matrix
- ROC Curve
- Model Performance Comparison

## Business Recommendations

- Implement real-time fraud detection using Machine Learning.
- Prioritize transactions with high anomaly scores.
- Combine behavioral indicators instead of relying on a single risk metric.
- Increase monitoring of Mobile App transactions.
- Deploy adaptive authentication for high-risk customers.
- Retrain fraud detection models periodically using new transaction data.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- Machine Learning
- Classification Algorithms
- Data Visualization

## Repository Structure

```text
banking-fraud-detection-machine-learning
│
├── Dataset
│   └── banking_transactions.csv
│
├── Notebooks
│   └── Banking_Fraud_Detection.ipynb
│
├── Python Scripts
│   └── fraud_detection.py
│
├── Images
│   ├── cover.png
│   ├── fraud_distribution.png
│   ├── boxplot_transaction_amount.png
│   ├── anomaly_distribution.png
│   ├── correlation_heatmap.png
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   ├── feature_importance.png
│   └── model_comparison.png
│
├── Documentation
│   ├── Model_Report.pdf
│   └── Business_Insights.pdf
│
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore
```

## Skills Demonstrated

- Machine Learning
- Predictive Analytics
- Exploratory Data Analysis
- Feature Engineering
- Classification Modeling
- Model Evaluation
- Data Visualization
- Fraud Detection
- Business Analytics
- Python Programming

## Future Improvements

- Train advanced boosting models such as XGBoost and LightGBM.
- Optimize hyperparameters using GridSearchCV.
- Address class imbalance using SMOTE.
- Build a real-time fraud prediction API.
- Deploy the model with Streamlit or Flask.
- Integrate Power BI dashboards for real-time monitoring.

## About This Project

This project was developed as part of my Data Analytics portfolio to demonstrate practical skills in Machine Learning, Predictive Analytics, Fraud Detection, Data Visualization, and Business Problem Solving.

If you found this project useful, consider giving it a ⭐ on GitHub.

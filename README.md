# Credit Default Risk Prediction & Customer Risk Segmentation

## 📌 Project Overview

This project develops an end-to-end **Credit Risk Analytics framework** using the **Home Credit Default Risk** dataset.

The objective is to predict the probability of customer default, identify key drivers of credit risk, segment customers into actionable risk categories, and support lending and underwriting decisions.

The project combines **data cleaning, exploratory data analysis, feature engineering, machine learning, risk analysis, and business interpretation** to simulate a real-world credit risk analytics workflow.

## 🎯 Business Problem

Financial institutions face significant losses when borrowers fail to repay their financial obligations.

This project focuses on:

* Predicting customer default risk
* Identifying key drivers of credit default
* Segmenting customers based on risk
* Supporting underwriting decisions
* Improving portfolio risk management
* Reducing expected credit losses
* Supporting more efficient credit allocation

The overall objective is to identify higher-risk applicants before or during the credit decision process and provide data-driven risk insights.

## 📊 Dataset

The project uses the **Home Credit Default Risk** dataset.

* **Observations:** 307,511 customers
* **Original variables:** 122
* **Target variable:** `TARGET`

### Target Definition

| TARGET | Meaning                                                  |
| ------ | -------------------------------------------------------- |
| `1`    | Customer experienced payment difficulties / default risk |
| `0`    | Customer did not experience payment difficulties         |

### Major Data Categories

The dataset contains information related to:

* Customer demographics
* Income
* Employment
* Housing
* Credit information
* Historical bureau information
* Behavioral and application characteristics

## 🔍 Exploratory Data Analysis

EDA was performed to understand customer characteristics and identify patterns associated with default risk.

Key analyses included:

* Overall default-rate analysis
* Age-based risk profiling
* Income-based risk profiling
* Occupation-level risk analysis
* Credit exposure analysis
* Customer characteristic comparisons

## 🧹 Data Cleaning

The data preparation process included:

* Removing variables with more than 50% missing values
* Missing-value treatment
* Duplicate checks
* Data consistency validation
* Categorical-variable standardization

A total of **41 variables with more than 50% missing values** were removed during the cleaning stage.

## ⚙️ Feature Engineering

Business-relevant credit-risk features were created to improve model representation and interpretability.

Key engineered variables included:

* **Age Years**
* **Income Groups**
* **Credit Groups**
* **Loan-to-Income Ratio**
* **Credit-to-Income Ratio**
* **Annuity Burden Ratio**
* **Employment Tenure**

These features were designed to represent borrower affordability, financial exposure, employment characteristics, and other factors relevant to retail credit underwriting.

## 🤖 Machine Learning Models

Three classification models were developed and compared:

### 1. Logistic Regression

Used as an interpretable classification approach and credit-risk baseline.

### 2. Random Forest

Used to capture nonlinear relationships and interactions through an ensemble of decision trees.

### 3. XGBoost

Used as a gradient-boosting approach for capturing more complex nonlinear patterns in the data.

## 📈 Model Evaluation

The models were evaluated using classification-performance measures including:

* ROC-AUC
* Precision
* Recall
* F1-score
* Confusion Matrix

Model comparison was used to assess predictive performance and understand the trade-off between model complexity, predictive power, and interpretability.

## 💳 Credit Risk Framework

The project is designed around concepts commonly used in credit-risk analytics, including:

* Probability of Default (PD)
* Credit scoring
* Risk segmentation
* WoE (Weight of Evidence)
* IV (Information Value)
* PSI (Population Stability Index)
* Model monitoring

Related credit-risk concepts such as **LGD, EAD, Basel III, and IFRS 9** are also considered as part of the broader credit-risk framework.

## 🏦 Business Applications

The framework can support financial institutions in:

* Identifying high-risk borrowers
* Improving underwriting decisions
* Prioritizing applications for manual review
* Allocating credit more efficiently
* Supporting risk-based pricing
* Managing portfolio risk
* Reducing expected credit losses

## 🛠️ Technology Stack

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **XGBoost**
* **LightGBM**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**

## 🔄 End-to-End Workflow

```text
Raw Loan Application Data
          ↓
Data Understanding
          ↓
Data Cleaning
          ↓
Exploratory Data Analysis
          ↓
Feature Engineering
          ↓
Data Preprocessing
          ↓
Class Imbalance Handling
          ↓
Model Development
          ↓
Logistic Regression
Random Forest
XGBoost
          ↓
Model Evaluation
          ↓
Risk Driver Analysis
          ↓
Credit Risk Interpretation
          ↓
Business Decision Support
```

## 📁 Project Structure

```text
Credit-Default-Risk-Prediction/
│
├── Credit Default Risk Prediction & Customer Risk Segmentation.ipynb
├── README.md
└── data/
    └── Loan_Application.csv
```

## 🚀 Key Learning Outcomes

This project demonstrates practical application of:

* Credit-risk analytics
* Exploratory data analysis
* Data cleaning
* Feature engineering
* Classification modeling
* Class-imbalance handling
* Model evaluation
* Risk-driver identification
* Credit-risk concepts
* Business-oriented model interpretation

## ⚠️ Disclaimer

This is an educational/project-based implementation using the Home Credit Default Risk dataset. It demonstrates credit-risk analytics concepts and should not be treated as a production lending decision system without appropriate validation, governance, regulatory compliance, fairness assessment, monitoring, and model-risk controls.


# Credit Card Fraud Detection

## Project Overview

This project develops a machine learning pipeline to detect fraudulent financial transactions using transaction-level data. The workflow includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and model serialization.

## Objectives

* Explore transaction data and fraud patterns.
* Perform exploratory data analysis.
* Engineer informative features.
* Build a fraud detection model.
* Evaluate classification performance.

## Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Joblib
* Jupyter Notebook

## Dataset

The dataset contains financial transaction records with features including transaction type, transaction amount, origin and destination balances, and fraud labels.

**Note:** The original dataset is not included in this repository because it exceeds GitHub's file size limit. A sample dataset or download link can be added separately.

## Project Workflow

### Data Exploration

* Inspected dataset structure.
* Checked missing values.
* Examined fraud distribution.
* Analyzed transaction types.
* Studied transaction amount distribution.

### Exploratory Data Analysis

Performed analysis on:

* Transaction type distribution
* Fraud rate by transaction type
* Transaction amount distribution
* Box plot of transaction amount by fraud class
* Top sender accounts
* Top receiver accounts
* Fraud analysis for TRANSFER and CASH_OUT transactions
* Correlation heatmap

### Feature Engineering

Created the following features:

* balanceDifforig
* balanceDiffdest

### Data Preprocessing

* Removed unnecessary columns
* Applied StandardScaler to numerical features
* Applied One-Hot Encoding to transaction type

## Machine Learning

Model Used

* Logistic Regression (class_weight="balanced")

Pipeline

* Train-Test Split
* Feature Scaling
* One-Hot Encoding
* Logistic Regression
* Model Evaluation

## Model Evaluation

Performance was evaluated using:

* Classification Report
* Confusion Matrix
* Accuracy Score

## Model Export

The trained model is saved as:

```text
credit_card_fraud_model.pkl
```

## Repository Structure

```text
Credit-Card-Fraud-Detection/
│
├── credit_cardfraud.ipynb
├── README.md
├── requirements.txt
├── credit_card_fraud_model.pkl
├── images/
└── sample_dataset.csv (optional)
```

## Installation

```bash
git clone <repository-link>

cd Credit-Card-Fraud-Detection

pip install -r requirements.txt
```

## Run

```bash
jupyter notebook credit_cardfraud.ipynb
```

Run all notebook cells sequentially.

## Future Improvements

* Compare multiple classification algorithms.
* Hyperparameter tuning.
* Improve fraud detection for highly imbalanced data.
* Deploy the model as a web application.

## Author

**Snigdha Singh**

Data Science | Machine Learning | Python

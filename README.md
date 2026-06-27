# 💳 Credit Card Fraud Detection

An end-to-end Machine Learning project that analyzes financial transaction data to detect fraudulent transactions. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, and a Logistic Regression model for fraud classification.

## 📌 Project Overview

Credit card fraud detection is a highly imbalanced classification problem where fraudulent transactions represent only a small fraction of all transactions. This project explores transaction patterns, engineers meaningful features, and builds a machine learning pipeline to classify fraudulent transactions.

## 🎯 Objectives

* Analyze transaction patterns and fraud distribution.
* Perform exploratory data analysis (EDA).
* Engineer balance-based features.
* Build a fraud detection model.
* Evaluate model performance using classification metrics.

## 🛠 Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Joblib
* Jupyter Notebook

## 📂 Dataset Features

The dataset includes:

* Transaction Type
* Transaction Amount
* Origin Account Balance
* Destination Account Balance
* Fraud Label (`isFraud`)
* Flagged Fraud (`isFlaggedFraud`)

## 📈 Project Workflow

### 1. Data Exploration

* Checked dataset structure and missing values.
* Analyzed fraud and flagged fraud distribution.
* Explored transaction types.
* Examined transaction amount distribution.

### 2. Exploratory Data Analysis

Performed analysis on:

* Transaction Type Distribution
* Fraud Rate by Transaction Type
* Transaction Amount Distribution (Log Scale)
* Amount vs Fraud (Box Plot)
* Top Senders and Receivers
* Fraud Distribution in **TRANSFER** and **CASH_OUT**
* Correlation Heatmap

### 3. Feature Engineering

Created new features:

* `balanceDifforig`
* `balanceDiffdest`

### 4. Data Preprocessing

* Removed unnecessary columns (`nameOrig`, `nameDest`, `isFlaggedFraud`)
* Standardized numerical features using **StandardScaler**
* Applied **One-Hot Encoding** to transaction type

## 🤖 Machine Learning Model

**Algorithm Used**

* Logistic Regression (`class_weight="balanced"`)

### Model Pipeline

* Train-Test Split
* Standard Scaling
* One-Hot Encoding
* Logistic Regression
* Model Evaluation

## 📊 Model Evaluation

Evaluated using:

* Classification Report
* Confusion Matrix
* Model Accuracy (`pipeline.score()`)

## 💾 Model Export

The trained model is saved as:

```text
credit_card_fraud_model.pkl
```

## 📁 Repository Structure

```text
Credit-Card-Fraud-Detection/
│
├── credit_cardfraud.ipynb
├── AIML Dataset.csv
├── credit_card_fraud_model.pkl
├── README.md
├── requirements.txt
└── images/
```

## ▶️ Installation

```bash
git clone <repository-link>

cd Credit-Card-Fraud-Detection

pip install -r requirements.txt
```

## 🚀 Run the Project

```bash
jupyter notebook credit_cardfraud.ipynb
```

Run all notebook cells sequentially.

## 📄 Conclusion

This project demonstrates the complete workflow of a fraud detection system, including data preprocessing, feature engineering, exploratory data analysis, and machine learning model development. A Logistic Regression classifier with balanced class weights was trained and evaluated to identify fraudulent financial transactions.

## 👨‍💻 Author

**Snigdha**

Data Analytics | Machine Learning | Python

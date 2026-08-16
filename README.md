# House Price Prediction using Linear Regression

A machine learning project that predicts house prices using Linear Regression on the Boston Housing dataset.

## 📌 Project Overview

This project demonstrates a basic end-to-end regression workflow using Python and Scikit-learn.

The workflow includes:

**Dataset Loading → Exploratory Data Analysis → Data Preprocessing → Train/Test Split → Linear Regression → Prediction → Visualization**

## 📊 Dataset

The project uses the Boston Housing dataset, loaded directly from the UCI Machine Learning Repository.

The dataset contains **505 records and 14 columns**, including 13 input features and the target variable `MEDV`.

### Features

- `CRIM`
- `ZN`
- `INDUS`
- `CHAS`
- `NOX`
- `RM`
- `AGE`
- `DIS`
- `RAD`
- `TAX`
- `PTRATIO`
- `B`
- `LSTAT`

### Target

- `MEDV` — Median value of owner-occupied homes

## 🔎 Exploratory Data Analysis

The dataset was explored using basic descriptive statistics and shape analysis.

Data quality was also checked for missing values and duplicate records.

Results:

- **Missing values:** 0
- **Duplicate records:** 0
- **Dataset shape:** 505 × 14

## 🧹 Data Preprocessing

The target variable `MEDV` was separated from the input features.

```python
X = df.drop("MEDV", axis=1)
y = df.iloc[:, -1].values

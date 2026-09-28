# Telco Customer Churn Analysis

## 📌 Project Overview

This project analyzes customer churn using the **Telco Customer Churn dataset** and builds two machine learning classification models:

* **Logistic Regression**
* **Random Forest Classifier**

The objective is to predict whether a customer is likely to churn (`Yes`) or remain with the company (`No`) and compare the performance of both models using standard classification metrics.

---

## 🎯 Project Objectives

* Explore and understand the Telco Customer Churn dataset.
* Clean and preprocess the data.
* Analyze customer churn patterns.
* Build a Logistic Regression model.
* Build a Random Forest Classifier.
* Evaluate both models using classification metrics.
* Identify important features associated with churn predictions.
* Compare the ability of both models to identify customers who churn.

---

## 📂 Dataset

**Dataset:** Telco Customer Churn

The dataset contains customer information related to:

* Customer demographics
* Account information
* Services subscribed
* Contract details
* Tenure
* Monthly charges
* Total charges
* Churn status

### Target Variable

`Churn`

* `Yes` → Customer churned
* `No` → Customer did not churn

---

## 🛠️ Technologies & Libraries

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

### Machine Learning Models

* Logistic Regression
* Random Forest Classifier

---

## 🔄 Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the Telco Customer Churn dataset.
2. Inspected the first five records.
3. Checked dataset dimensions.
4. Checked data types.
5. Identified missing values.
6. Converted `TotalCharges` to a numerical datatype.
7. Handled missing values in `TotalCharges`.
8. Removed `customerID` because it is an identifier and does not provide useful predictive information.
9. Encoded categorical variables using one-hot encoding.
10. Converted the target variable `Churn` into binary values:

* `No = 0`
* `Yes = 1`

11. Split

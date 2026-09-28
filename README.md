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

11. Split the data into 80% training and 20% testing datasets.
📊 Exploratory Data Analysis

The analysis examined:

Customer Churn Percentage

The percentage of customers who churned was calculated to understand the overall churn level in the dataset.

Average Monthly Charges

Average MonthlyCharges were compared between:

Churn = No
Churn = Yes
Average Tenure

Average customer tenure was compared between:

Churn = No
Churn = Yes

These comparisons help identify differences in customer behavior between churned and non-churned customers.

🤖 Machine Learning Models
1. Logistic Regression

A Logistic Regression model was trained to predict the probability of customer churn.

Evaluation Metrics

The model was evaluated using:

Accuracy
Precision
Recall
F1-score
Confusion Matrix
Classification Report
Feature Analysis

The absolute values of the Logistic Regression coefficients were used to identify the top 5 features associated with the model's churn predictions.

A positive coefficient indicates an association with a higher predicted probability of Churn = Yes, while a negative coefficient indicates an association with a lower predicted probability.

2. Random Forest Classifier

A Random Forest Classifier was trained using:

n_estimators = 100
random_state = 42

The model was evaluated using:

Accuracy
Precision
Recall
F1-score
Confusion Matrix
Classification Report
Feature Importance

Random Forest feature importance was used to identify the top 10 features contributing to the model's predictions.

The top three features were further examined to understand which customer characteristics were most useful to the model when distinguishing churned and non-churned customers.

📈 Model Comparison

The performance of Logistic Regression and Random Forest was compared using:

Metric	Logistic Regression	Random Forest
Accuracy	Calculated in notebook	Calculated in notebook
Precision	Calculated in notebook	Calculated in notebook
Recall	Calculated in notebook	Calculated in notebook
F1-score	Calculated in notebook	Calculated in notebook

The recall for the Churn = Yes class was specifically compared because it measures how many of the customers who actually churned were correctly identified by the model.

🔍 Confusion Matrix Analysis

For the Random Forest model, the confusion matrix was used to identify:

True Positive (TP): Customers correctly predicted as churned.
False Positive (FP): Customers incorrectly predicted as churned.
False Negative (FN): Customers who actually churned but were predicted as non-churned.
True Negative (TN): Customers correctly predicted as non-churned.

This provides a detailed view of the model's classification performance.

💡 Key Insights

The analysis provides the following types of business insights:

The overall percentage of customers who churned provides an understanding of the churn level in the customer base.
Comparing average monthly charges helps identify differences in billing patterns between churned and non-churned customers.
Comparing average tenure helps identify differences in customer retention duration.
Logistic Regression coefficients provide an interpretable view of features associated with churn predictions.
Random Forest feature importance identifies characteristics that were particularly useful to the model for predicting churn.
Comparing recall for Churn = Yes helps evaluate how effectively the models identify customers who actually churned.

Note: Feature importance and model coefficients describe relationships used by the models for prediction; they should not be interpreted as proof that a particular characteristic causes customer churn.

📁 Project Structure
Telco-Customer-Churn-Analysis/
│
├── Telco_Customer_Churn_Analysis.ipynb
│
├── data/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── images/
│   ├── confusion_matrix_logistic.png
│   ├── confusion_matrix_random_forest.png
│   └── feature_importance.png
│
└── README.md
▶️ How to Run the Project
1. Clone the repository
git clone <your-github-repository-url>
2. Navigate to the project folder
cd Telco-Customer-Churn-Analysis
3. Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
4. Start Jupyter Notebook
jupyter notebook
5. Open
Telco_Customer_Churn_Analysis.ipynb

Run the notebook cells sequentially.

📌 Conclusion

This project demonstrates an end-to-end machine learning workflow for customer churn prediction, including data exploration, preprocessing, feature encoding, model training, evaluation, feature analysis, and model comparison.

The project provides practical experience with Python, Pandas, data preprocessing, exploratory data analysis, Logistic Regression, Random Forest, classification metrics, confusion matrices, and feature importance.

👨‍💻 Skills Demonstrated

Python | Pandas | NumPy | Matplotlib | Seaborn | Scikit-learn | EDA | Data Preprocessing | Logistic Regression | Random Forest | Classification | Feature Importance | Model Evaluation

📘 Project Overview
Title: Telco-Customer-Churn Prediction

Objective:
The primary aim of this project was to develop a predictive model that can accurately identify customers who are likely to churn (discontinue services) in a telecommunications company. By leveraging customer demographics, service usage patterns, and account information, the goal was to provide actionable insights that can help in formulating targeted retention strategies.

Dataset:
The analysis was conducted using the Telco Customer Churn dataset, which contains information about 64,374 customers across 15 features. These features encompass customer demographics, service usage, and account details, with the target variable being 'Churn', indicating whether a customer has left the company.

🔍 Data Preprocessing & Exploration
Initial Steps:

Data Loading:
The dataset was loaded into a Pandas DataFrame for initial inspection and analysis.

Feature Inspection:
The dataset comprises the following columns:

Column Name	Description
CustomerID	= Unique identifier for each customer
Age	= Age of the customer
Gender	= Gender of the customer
Tenure	= Number of months the customer has been with the company
Usage Frequency	= Frequency of service usage
Support Calls	= Number of support calls made by the customer
Payment Delay =	Delay in payment (if any)
Subscription Type =	Type of subscription (e.g., monthly, yearly)
Contract Length	= Duration of the contract
Total Spend =	Total expenditure by the customer
Last Interaction	= Time since the last interaction with the customer
Churn =	Target variable indicating customer churn (1 = Yes, 0 = No)

Data Cleaning:

Missing Values:
Identified and handled missing values appropriately to ensure data integrity.

Data Type Conversion:
Converted categorical variables into numerical formats using encoding techniques.

Feature Scaling:
Standardized numerical features to bring them to a common scale, enhancing model performance.

📊 Exploratory Data Analysis (EDA)
Churn Distribution:
Analyzed the distribution of the target variable 'Churn' to understand the balance between churned and retained customers.

Correlation Analysis:
Investigated correlations between numerical features to identify potential relationships and multicollinearity.

Feature Importance:
Utilized techniques like Recursive Feature Elimination (RFE) to rank features based on their importance in predicting churn.

🤖 Model Development
Model Selection:
Several machine learning models were trained and evaluated to predict customer churn:

Logistic Regression:
A statistical model used for binary classification tasks.

K-Nearest Neighbors (KNN):
A non-parametric method used for classification based on distance metrics.

Decision Tree Classifier:
A model that splits data into subsets based on feature values, forming a tree-like structure.

Random Forest Classifier:
An ensemble method that constructs multiple decision trees and merges their outputs for improved accuracy.

Model Evaluation Metrics:

Accuracy:
The proportion of correctly predicted instances.

AUC (Area Under the Curve):
A performance measurement for classification problems at various thresholds settings.

Recall:
The ability of the model to identify all relevant instances (true positives).

Precision:
The ability of the model to identify only relevant instances (true positives).

F1-Score:
The weighted average of Precision and Recall.



Results:

Logistic Regression:

Accuracy: 77.3%

AUC: 0.8614

Recall: 83.86%

Precision: 74.14%

F1-Score: 78.7%



KNN:

Accuracy: 77.43%

AUC: 0.825

Recall: 68.09%

Precision: 83.73%

F1-Score: 75.1%



Decision Tree Classifier:

Accuracy: 95.69%

AUC: 0.9569

Recall: 95.73%

Precision: 95.65%

F1-Score: 95.69%



Random Forest Classifier:

Accuracy: 96.26%

AUC: 0.9962

Recall: 94.38%

Precision: 98.07%

F1-Score: 96.19%

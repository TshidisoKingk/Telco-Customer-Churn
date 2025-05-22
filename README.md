# Telco-Customer-Churn
Telco Customer Churn Prediction: A Comprehensive Analysis and Model Evaluation
Project Overview
Customer churn is a critical issue in the telecommunications industry, where retaining existing customers is more cost-effective than acquiring new ones. This project aims to predict customer churn for a telecom company using machine learning techniques, enabling proactive retention strategies.

Dataset
The dataset used in this project is the Telco Customer Churn dataset, which contains information about 60,986 customers. The features include:

Demographics: Gender, SeniorCitizen, Partner, Dependents

Account Information: Tenure, Contract, PaperlessBilling, PaymentMethod

Service Usage: MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies

Billing Information: MonthlyCharges, TotalCharges

Target Variable: Churn (Yes/No)

Data Preprocessing
The data underwent several preprocessing steps:

Handling Missing Values: Missing values were identified and appropriately handled.

Encoding Categorical Variables: Categorical variables were encoded into numerical values for model compatibility.

Feature Scaling: Numerical features were scaled to ensure consistent ranges, improving model performance.

Exploratory Data Analysis (EDA)
EDA revealed key insights:

Churn Distribution: The dataset is balanced, with an equal number of churned and non-churned customers.

Feature Correlations: Strong correlations were found between features like MonthlyCharges and TotalCharges, and the target variable Churn.

Model Development
Several machine learning models were implemented and evaluated:

Logistic Regression
Accuracy: 77.3%

AUC: 0.8614

Recall: 83.86%

Precision: 74.14%

F1-Score: 78.7%

Average Precision-Recall Score: 85.89%

K-Nearest Neighbors (KNN)
Accuracy: 77.43%

AUC: 0.825

Recall: 68.09%

Precision: 83.73%

F1-Score: 75.1%

Average Precision-Recall Score: 85.49%

Decision Tree Classifier
Accuracy: 95.69%

AUC: 0.9569

Recall: 95.73%

Precision: 95.65%

F1-Score: 95.69%

Average Precision-Recall Score: 93.7%

Random Forest Classifier
Accuracy: 96.26%

AUC: 0.9962

Recall: 94.38%

Precision: 98.07%

F1-Score: 96.19%

Average Precision-Recall Score: 99.63%

Model Evaluation
The Random Forest Classifier outperformed other models in terms of accuracy, AUC, and F1-Score. However, the high accuracy suggests potential overfitting, possibly due to class imbalance or data leakage.

# Customer Retention Analytics

## Project Summary

Customer churn is a major challenge for telecommunication companies, as retaining existing customers is more cost-effective than acquiring new ones. This project uses the IBM Telco Customer Churn dataset to predict whether a customer is likely to churn based on demographic, account, service, and billing information. Multiple machine learning models were developed and compared to identify the most effective solution for churn prediction.

## Requirement

Telecommunication companies need to identify customers who are likely to leave so that proactive retention strategies can be implemented. The objective of this project is to build a predictive machine learning model that helps reduce customer churn, improve customer satisfaction, and support data-driven business decisions.

## Project Goal

* Predict customer churn using supervised machine learning.
* Identify the key factors influencing churn.
* Compare the performance of multiple classification models.
* Select the best-performing model for churn prediction.
* Generate business insights and recommendations to improve customer retention.

## Analysis

The dataset was examined for data quality, missing values, duplicates, and feature distributions. The `customerID` column was removed as it is a unique identifier, while missing values in `TotalCharges` were handled after converting the column to a numeric data type.

Exploratory Data Analysis (EDA) was performed using visualizations to understand customer behavior and churn patterns. Categorical variables were encoded using One-Hot Encoding, the target variable (`Churn`) was converted to binary values, and numerical features were standardized where required.

Seven classification models were trained and evaluated: Logistic Regression, Decision Tree, Random Forest, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), XGBoost, and Artificial Neural Network (ANN). Model performance was assessed using Accuracy, Precision, Recall, F1-Score, Confusion Matrix, and ROC-AUC.

## Summary & Results

The performance of the models is summarized below:

| Model                           |   Accuracy |
| ------------------------------- | ---------: |
| **Logistic Regression**         | **80.70%** |
| Support Vector Machine (SVM)    |     79.28% |
| Random Forest                   |     78.99% |
| XGBoost                         |     78.21% |
| Artificial Neural Network (ANN) |     77.22% |
| K-Nearest Neighbors (KNN)       |     74.73% |
| Decision Tree                   |     72.75% |

Logistic Regression achieved the highest accuracy (**80.70%**) and was selected as the final model.

The analysis showed that **longer customer tenure**, **one-year and two-year contracts**, **Online Security**, and **Tech Support** reduced churn, while **Fiber Optic Internet**, **Electronic Check payment**, and certain billing characteristics increased the likelihood of customer churn.

## Recommendations

* Encourage customers to switch to long-term contracts through incentives and loyalty programs.
* Improve service quality and customer experience for Fiber Optic users.
* Strengthen customer engagement during the early stages of the customer lifecycle.
* Promote value-added services such as Tech Support and Online Security.
* Encourage customers to use more stable payment methods instead of Electronic Check.
* Use the predictive model to identify high-risk customers and implement proactive retention campaigns.
* Continuously monitor model performance and retrain it using updated customer data to maintain prediction accuracy.

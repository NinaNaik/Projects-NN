IBM Telco Customer Churn Dataset

This project builds an end-to-end machine learning pipeline that predicts which telecom customers are likely to leave the service, enabling businesses to proactively target retention campaigns and reduce customer attrition. Using the IBM Telco Customer Churn dataset, the solution combines exploratory data analysis, feature engineering, model comparison, and hyperparameter optimization to deliver strong predictive performance with a ROC-AUC of 0.889.
Technical Architecture & Approach
Data Pipeline Dataset
IBM Telco Customer Churn Dataset 
Customer demographics, service subscriptions, billing information, contract details, and churn labels. 
Workflow
Raw Customer Data
Data Cleaning & Validation
Exploratory Data Analysis (EDA)
Feature Engineering
Preprocessing Pipeline
 ├─ Standard Scaling (Numerical Features)
 └─ One-Hot Encoding (Categorical Features)
Train/Test Split
Model Training
 ├─ Logistic Regression
 ├─ Random Forest
 └─ XGBoost
Stratified K-Fold Cross Validation
GridSearchCV Hyperparameter Tuning
Final Evaluation on Hold-Out Test Set
Model Selection
Three supervised learning algorithms were evaluated:
Model	Purpose
Logistic Regression	Baseline interpretable model
Random Forest	Ensemble tree-based benchmark
XGBoost	High-performance gradient boosting model
The final solution selected XGBoost due to its superior ROC-AUC performance during cross-validation and testing.
Machine Learning Techniques Used
•	Exploratory Data Analysis (EDA) 
•	Feature Importance Analysis 
•	One-Hot Encoding 
•	Feature Scaling 
•	Stratified K-Fold Cross Validation 
•	GridSearchCV Hyperparameter Optimization 
•	Pipeline-based preprocessing to prevent data leakage 

Final Test Performance
Metric	Score
Accuracy	83%
ROC-AUC	0.889
Churn Precision	72%
Churn Recall	59%
Churn F1-Score	0.65
Classification Report
Class	Precision	Recall	F1-Score
Non-Churn	0.86	0.92	0.89
Churn	0.72	0.59	0.65



AMAZON DATASET: 

Built an end-to-end Amazon electronics analytics and machine learning pipeline using Python, Pandas, Scikit-learn, and Random Forest Regression to analyze pricing trends, perform exploratory data analysis, and predict product prices from customer engagement metrics.

Technical Architecture & Approach
Data Pipeline
Raw Amazon Electronics Dataset
 Data Cleaning (Missing Values, Duplicates)
 Exploratory Data Analysis (Distributions, Outliers, Correlation Analysis)
 Feature Engineering & Data Preparation
 Train/Test Split (80/20)
 Feature Scaling  (StandardScaler)
 Random Forest Regressor
 Model Evaluation ( Mean Squared Error)

Model Selection
•	Evaluated regression-based prediction workflow. 
•	Implemented a Random Forest Regressor due to: 
o	Ability to capture non-linear relationships. 
o	Robustness against noisy e-commerce data. 
o	Better handling of feature interactions compared to simple linear models. 
Machine Learning Performance
Metric	Value
Mean Squared Error (MSE)	72,607,294.33

Interpretation
•	The Random Forest model successfully learned pricing patterns from available product features. 
•	The model provides a baseline framework for price prediction and can be further improved through: 
o	Additional feature engineering. 
o	Hyperparameter tuning. 
o	Inclusion of product category and text-based features. 
o	Advanced ensemble techniques. 


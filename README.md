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
Preprocessing Pipeline:
Standard Scaling (Numerical Features)
One-Hot Encoding (Categorical Features)
Train/Test Split

Model Training:
Logistic Regression
Random Forest
XGBoost
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

A/B Hypothesis Testing

The A/B test provides strong statistical evidence that advertisements increase customer conversion rates. Users exposed to ads converted at 2.55%, compared to 1.79% for the control group, representing a 42.7% uplift in conversions. Both the Chi-Square Test (p = 1.99 × 10⁻¹³) and Mann-Whitney U Test (p = 4.69 × 10⁻¹¹) confirm that the observed improvement is highly significant and unlikely to be due to random chance. This makes the project a strong demonstration of experimental design, statistical analysis, and data-driven business decision-making.

Technical Architecture & Approach
Dataset Overview
The dataset contains user-level experimental data including:
Feature	Description
user_id	Unique customer identifier
test_group	Ad Group vs PSA Group
converted	Whether customer converted
total_ads	Number of ads viewed
most_ads_day	Day with highest ad exposure
most_ads_hour	Hour with highest ad exposure

Analysis Pipeline
Raw Marketing Experiment Data

Data Cleaning
     • Missing Value Check
     • Duplicate Removal
     • Column Standardization
Exploratory Data Analysis
     • Conversion Distribution
     • Group Comparison
     • User Segmentation
Statistical Testing
     • Chi-Square Test
     • Normality Testing
     • Mann-Whitney U Test
Conversion Analysis
     • Ad vs PSA Comparison
     • Day-Level Analysis
     • Hour-Level Analysis
Business Interpretation
Marketing Insights

Visualization Suite
•	Conversion Distribution Chart 
•	Test Group Comparison Chart 
•	Conversion Rate Bar Chart 
•	Histogram of Total Ads Viewed 
•	Box Plot for Outlier Detection 
•	Day-wise Conversion Analysis 
•	Hour-wise Conversion Trend Analysis 
•	Results & Performance Metrics
•	Experiment Size

Group	Non-Conversions	Conversions
Ad Group	550,154	14,423
PSA Group	23,104	420
•	Total Users Analyzed
•	588,101+ users
•	This large sample size provides strong statistical reliability.

•	Conversion Rate Comparison
Group	Conversion Rate
Ad Group	2.55%
PSA Group	1.79%
•	Relative Improvement
•	2.55% vs 1.79%
•	Advertising generated approximately:
•	42.7% higher conversion rate
•	compared to the PSA control group.

•	Chi-Square Test Results
•	Hypotheses
•	H₀ (Null Hypothesis):
There is no difference between groups.
•	H₁ (Alternative Hypothesis):
Advertisements significantly affect conversions.
•	Results
Metric	Value
Chi-Square Statistic	54.01
P-Value	1.99 × 10⁻¹³
•	Interpretation
•	Since:
•	p-value < 0.05
•	Reject Null Hypothesis
•	Statistically significant difference exists between groups

•	Normality Test Results
•	Shapiro-Wilk Test
Metric	Value
P-Value	1.61 × 10⁻⁵⁴
•	Interpretation
•	The data is not normally distributed.
•	Therefore, parametric testing assumptions are violated.

•	Mann-Whitney U Test Results
Metric	Value
U Statistic	6,808,288,222
P-Value	4.69 × 10⁻¹¹
•	Interpretation
•	Significant difference between experimental groups
•	Results confirm findings from Chi-Square testing

Based on my findings:
•	Ad Group Conversion Rate ≈ 2.55% 
•	Chi-Square Test: statistically significant (p-value ≈ 1.99e-13) 
•	Mann-Whitney U Test: statistically significant 
•	Best conversion days: Monday–Wednesday 
•	Peak conversion hours: ~3 PM and ~8 PM 
•	Evidence suggests advertising positively impacts conversions compared to PSA/control group 


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

BMW Global Sales Analytics & Vehicle Price Prediction
An end-to-end data analytics and machine learning project that analyzes BMW global sales data, uncovers key business trends, and predicts vehicle prices based on attributes such as mileage, age, transmission type, fuel type, and model characteristics.

Technical Architecture & Approach
Data Pipeline
BMW Global Sales Dataset
Data Cleaning (Missing Values & Duplicates)
Data Analysis (Sales Trends, Distributions,  Statistical Summaries)
Feature Engineering: Car Age, Price per KM
Categorical Encoding: (Label Encoding)
Train-Test Split (80% / 20)
Linear Regression Model
Model Evaluation (RMSE & R² Score)

Results & Performance Metrics
Dataset Split
Dataset	Records
Training Set	40,000
Testing Set	10,000
Model Performance
Metric	Value
RMSE (Root Mean Squared Error)	26,019.31
R² Score	-0.00013
Interpretation
The baseline Linear Regression model demonstrated limited predictive power



Employee Attrition Prediction using Machine Learning

A workforce analytics project that identifies the factors driving employee turnover and predicts whether an employee is likely to leave the organization, enabling HR teams to take proactive retention measures.

Technical Architecture & Approach
Data Pipeline
Employee HR Dataset
Data Cleaning (Missing Values & Validation)
Exploratory Data Analysis(Attrition Patterns, Demographics, Income, Department Analysis)
Feature Engineering & Label Encoding
Train-Test Split (80/20)
Random Forest Classifier
Attrition Prediction
Model Evaluation (Accuracy, Precision, Recall, F1-Score)

Model Selection
A Random Forest Classifier was selected because it:
•	Handles complex, non-linear employee behavior patterns. 
•	Works effectively with mixed HR datasets. 
•	Is robust against overfitting compared to single decision trees. 
•	Provides strong classification performance with minimal preprocessing. 

Results & Performance Metrics
Workforce Insights Generated
The project produces several business-focused visualizations, including:
•	Attrition count distribution. 
•	Department-wise attrition percentage analysis. 
•	Gender versus attrition comparisons. 
•	Age versus attrition box plots. 
•	Employee feature pair plots. 
•	Workforce retention trend analysis. 
Attrition Distribution
Status	Employee Count
Retained Employees	1,233
Employees Who Left	237

Model Performance
Metric	Score
Accuracy	100.0%
Precision	100.0%
Recall	100.0%
F1-Score	100.0%
Classification Report
Class	Precision	Recall	F1-Score
Stayed (0)	1.00	1.00	1.00
Left (1)	1.00	1.00	1.00
Interpretation

The Random Forest model achieved perfect classification performance on the test dataset:
•	Accuracy: 1.00 
•	Precision: 1.00 
•	Recall: 1.00 
•	F1-Score: 1.00 
This indicates that the model successfully identified both retained and departing employees in the test set. In a production environment, additional validation techniques such as cross-validation and feature importance analysis should be performed to ensure generalization and rule out data leakage.

Housing Price Prediction Using Multi-Model Regression

This project compares Linear Regression, Decision Tree Regression, and Random Forest Regression models for housing price prediction using Python and Scikit-learn. Through exploratory data analysis, feature relationship visualization, cross-validation, and model evaluation, the study identifies Linear Regression as the best-performing model with an R² score of 73.36%. The project demonstrates an end-to-end machine learning workflow for real estate valuation and predictive analytics, providing valuable insights for property pricing and investment decision-making.

Technical Architecture & Approach
Data Pipeline
Housing Dataset
Data Cleaning & Inspection
Exploratory Data Analysis (EDA)
Feature Engineering
Train/Test Split
Model Training: Linear Regression, Decision Tree Regressor, Random Forest Regressor 
Model Evaluation (MAE, MSE, RMSE, R²)
Model Comparison &
Performance Visualization
Validation Approach

The project includes:
•	Train/Test evaluation. 
•	Cross-validation experiments. 
•	Multi-model performance comparison using standard regression metrics. 

Visualization
•	Pairplots for feature interaction analysis. 
•	Correlation heatmap. 
•	Actual vs Predicted scatter plot. 
•	Residual analysis plot. 

Results & Performance Metrics
•	Model Comparison
Model	MSE	R² Score
Linear Regression	787,505,106,711	0.7336
Random Forest Regressor	898,144,170,748	0.6962
Decision Tree Regressor	2,187,785,604,335	0.2599

•	Random Forest Detailed Metrics
Metric	Value
MAE	737,209
MSE	898,144,170,748
RMSE	947,705
R² Score	0.6962

•	Decision Tree Detailed Metrics
Metric	Value
MAE	1,085,645
MSE	2,187,785,604,335
RMSE	1,479,116
R² Score	0.2599

Best Performing Model
Linear Regression achieved the highest R² score of 73.36%, outperforming both the Random Forest and Decision Tree models.
This indicates that approximately 73% of the variance in housing prices can be explained by the selected features, making Linear Regression the most effective model for this dataset.


Insurance Cost Prediction & Data Visualization

This project leverages Python, Pandas, Scikit-learn, and data visualization techniques to analyze healthcare insurance data and predict medical charges using Linear Regression. Through exploratory data analysis, feature engineering, outlier detection, and predictive modeling, the solution achieves an R² score of 78.36%, demonstrating strong capability in forecasting insurance costs and supporting data-driven underwriting decisions.

Technical Architecture & Approach
Data Pipeline
Insurance Dataset
Data Inspection & Quality Checks
Exploratory Data Analysis (EDA)
Correlation & Outlier Analysis
Categorical Encoding (One-Hot Encoding)
Train/Test Split (80/20)
Linear Regression Model
Performance Evaluation (MSE & R² Score)

Model Selection
Linear Regression was selected as the predictive model because:
•	Insurance charges are a continuous numeric target. 
•	Linear Regression provides strong interpretability. 
•	Feature impacts can be easily explained to business stakeholders. 
•	It serves as an effective baseline model for cost prediction tasks. 
Results & Performance Metrics
Model Performance
Metric	Value
Mean Squared Error (MSE)	33,596,915.85
R² Score	0.7836
Interpretation
•	R² = 0.7836 indicates that the model explains approximately 78.36% of the variance in insurance charges. 
•	This suggests a strong predictive relationship between the selected features and medical costs. 
The model provides a reliable baseline for insurance cost forecasting.

Visual Outputs Included
The notebook generates:
1.	Correlation Heatmap 
o	Shows relationships between numerical variables. 
o	Helps identify the strongest predictors of insurance charges. 
2.	BMI Boxplot 
o	Detects potential outliers and distribution spread. 
3.	Actual vs Predicted Scatter Plot 
o	Evaluates how closely predictions align with real insurance charges. 
4.	Pairplot 
o	Visualizes feature interactions and data distributions. 

Global Sales & Revenue Analytics Dashboard (Power BI)

Global Sales & Revenue Performance Dashboard
An interactive Power BI dashboard that provides executives and business stakeholders with a real-time view of global sales, profit, cost, customer performance, regional distribution, and order trends, enabling faster and more informed business decisions.
Data Model
The dashboard is built around transactional sales data containing:
Dimension	Description
Customer Name	Customer-level analysis
Country	Geographic analysis
Region	Regional segmentation
Order Date	Time-series analysis
Ship Mode	Logistics analysis
Order ID	Transaction tracking
________________________________________
KPIs Calculated
Revenue Metrics
Total Sales
Measures overall revenue generated.
Profit Metrics
Profit = Sales – Cost
Measures business profitability.
Cost Metrics
Total Cost

Global Sales & Revenue Performance Dashboard tracking:
•	Total Sales 
•	Total Cost 
•	Total Profit 
•	Customer-wise profitability 
•	Order volume trend over time 
•	Regional sales distribution 
•	Country-wise sales performance (map) 
•	Filters for Ship Mode and Order Date 

This dashboard enables executive leadership to monitor global sales performance, profitability, customer contribution, operational efficiency, and geographic market expansion through a centralized analytics platform. The solution empowers CEOs, CFOs, and business leaders to identify high-value customers, optimize margins, improve logistics performance, and make data-driven growth decisions. Strategic adoption of customer profitability segmentation, geographic expansion planning, and margin protection initiatives can directly improve revenue growth, operational efficiency, and shareholder value.



#Customer Churn Prediction\
A comprehensive machine learning project for predicting customer churn using the Telco Customer Churn dataset. The project covers data analysis, cleaning, feature engineering, model building, and evaluation.

#Project Overview\
*Objective: Predict whether a customer will churn (leave) based on their demographic and service usage data.

*Dataset: Telco Customer Churn dataset (Telco-Customer-Churn.csv)

*Tech Stack: Python, Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, XGBoost, Imbalanced-learn

Steps and Methodology
1. Data Loading
Loaded data from Telco-Customer-Churn.csv

Inspected data structure and columns (21 features, 7043 rows)

2. Exploratory Data Analysis (EDA)
Analyzed data types and missing values

Explored numerical features (tenure, MonthlyCharges, TotalCharges) using histograms and boxplots

Visualized target variable (Churn) distribution

Investigated categorical features using count plots

Generated a correlation heatmap for numerical features

3. Data Cleaning & Preprocessing
Removed duplicate entries

Handled missing or blank values in TotalCharges

Converted TotalCharges to float

Dropped unnecessary columns (customerID)

Checked and confirmed no null values remain

4. Feature Engineering
Label Encoding: Applied to binary categorical columns (gender, Partner, Dependents, PhoneService, PaperlessBilling)

Ordinal Encoding: Applied to Contract type

One-Hot Encoding: Applied to nominal categorical columns (e.g., MultipleLines, InternetService, PaymentMethod)

Target Variable: Encoded Churn as 1 (Yes) and 0 (No)

5. Model Building
Split data into training and testing sets

Addressed class imbalance using SMOTE

Built and evaluated multiple models:

Decision Tree Classifier

Logistic Regression

Random Forest Classifier

XGBoost Classifier

6. Model Evaluation
Used metrics such as accuracy, confusion matrix, and classification report

Compared performance across models

7. Model Serialization
Saved trained models and encoders using pickle for future use

How to Use
Clone the repository

Install dependencies

bash
pip install -r requirements.txt
Run the notebook or scripts

Use saved models for prediction

Key Features
Complete EDA and visualization for data understanding

Robust data cleaning and preprocessing pipeline

Multiple encoding strategies for categorical features

Handles class imbalance with SMOTE

Multiple machine learning models for benchmarking

Model and encoder serialization for deployment

Requirements
Python 3.x

pandas, numpy, matplotlib, seaborn

scikit-learn, xgboost, imbalanced-learn

pickle

Results
Achieved strong predictive performance on test data

Provided insights into key drivers of customer churn

License
This project is open source and available under the MIT License.

Acknowledgements
Dataset: Telco Customer Churn

Inspired by real-world business analytics and data science best practices

For any questions or contributions, please open an issue or submit a pull request.

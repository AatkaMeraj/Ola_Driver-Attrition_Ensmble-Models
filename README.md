# Ola_Driver-Attrition using Ensmble Models

📌 Project Overview

This project analyzes driver attrition at Ola, identifying key factors influencing driver retention and churn. Using EDA, feature engineering, and machine learning, we aim to predict whether a driver is likely to leave the company, helping optimize workforce management.

🛠️ Technologies Used

Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)

SQL (for data preprocessing and aggregation)

Machine Learning (Random Forest, XGBoost, Gradient Boosting)

📊 Data Processing & Feature Engineering

Handled missing values using KNN imputation.

Aggregated driver data to remove duplicates using groupby and aggregations.

Created new features:

Quarterly rating increase: 1 if rating improved, else 0.

Monthly income increase: 1 if salary increased, else 0.

Target variable: 1 if the driver left the company, else 0.

One-hot encoding for categorical variables.

Standardized numerical features using MinMaxScaler.

📈 Key Insights

816 drivers saw an increase in quarterly ratings.

Only 43 drivers experienced a salary hike.

Attrition rate: Nearly 50% of drivers left the company.

Most drivers joined mid-year rather than at the start or end.

Peak hiring trend: More drivers joined as the years progressed.

Gender & Income: Male drivers earned slightly more than females.

🔍 Model Performance

Trained ensemble models to predict driver attrition such as Random Forest, XG Boost and Gradient Boost, and the performance are as follows:

Without SMOTE

Random Forest: F1-score (Stayed: 0.94, Left: 0.81)

XGBoost: F1-score (Stayed: 0.95, Left: 0.86)

Gradient Boosting: F1-score (Stayed: 0.95, Left: 0.85)

With SMOTE

Random Forest: F1-score (Stayed: 0.92, Left: 0.81)

XGBoost: F1-score (Stayed: 0.93, Left: 0.81)

Gradient Boosting: F1-score (Stayed: 0.92, Left: 0.81)

🚀 Results & Impact

Best performing model: XGBoost with an F1-score of 86% for predicting attrition.

Feature importance analysis helped identify key factors influencing attrition.

Data-driven strategies can improve driver retention and workforce management.


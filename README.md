# Bank-Customer-Segmentation-Targeted-Marketing-model

## 🧠 Project Overview
This project aims to segment credit card customers into distinct groups using unsupervised machine learning, specifically KMeans clustering, to assist financial institutions in crafting targeted marketing strategies, improving customer engagement, and reducing churn.

## 📌 Objectives
- Perform end-to-end customer segmentation using clustering.

- Engineer meaningful features from raw financial attributes.

- Compare multiple scaling techniques and evaluate clustering quality.

- Profile each customer segment with actionable business insights.

## 🗃️ Dataset Summary
- Source: Kaggle (Credit Card Dataset for Clustering)

- Rows: 8,950 | Columns: 18

- Target Variable: None (unsupervised learning)

- Key Features: BALANCE, PURCHASES, PAYMENTS, CREDIT_LIMIT, etc.

## 🔧 Tools & Technologies

- Pandas, NumPy – Data Cleaning & Preprocessing

- Matplotlib, Seaborn – Data Visualization

- Scikit-learn – Feature Scaling & Clustering

- Silhouette Score – Clustering Evaluation

## 📊 Key Steps
- EDA & Data Cleaning

Detected and handled missing values

Removed irrelevant columns (e.g., CUST_ID)

Explored skewness, kurtosis, and outliers

- Feature Engineering

Derived meaningful ratios (e.g., CASH_USAGE_RATIO, PAYMENT_RATIO)

Created ACTIVITY_INDEX as an overall usage indicator

- Scaling Comparison

Tested StandardScaler, MinMaxScaler, and RobustScaler

Also compared with log-transformed data and no-scaling baseline

Evaluated performance using Silhouette Score

- Final Model Selection

Chose 3 clusters on the cleaned dataset without scaling

This version offered a balance of high silhouette score and better interpretability

Customer Profiling

Identified strategic personas for each segment

Developed insights for marketing, risk management, and retention

## 📌 Key Results
Approach	Clusters	Silhouette Score
Cleaned + MinMax	2	~25
Cleaned (No Scaling)	2	45
Cleaned (No Scaling)	3	44 ✅
Log Transformed	8	47

## Final Choice: Cleaned Dataset (No Scaling) with 3 Clusters

🔍 Business Impact
🎯 Segmented Customers for more targeted credit card offers

💼 Identified Outliers for risk analysis and fraud monitoring

📈 Enhanced Customer Understanding for strategic decision-making

## Folder Structure
project/
│
├── data/
│   └── raw, processed/
│
├── notebooks/
│   └── EDA.ipynb
│   └── Feature_Engineering.ipynb
│   └── Clustering_Evaluation.ipynb
│   └── Customer_Profiling.ipynb
│
├── outputs/
│   └── Charts, Cluster Plots
    └──model
│
├── README.md
## 📬 Let's Connect
- 📌 Connect on LinkedIn : https://www.linkedin.com/in/sudais-shah-938b9a312/

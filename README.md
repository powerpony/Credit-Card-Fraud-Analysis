# Credit-Card-Fraud-Analysis
## Project Overview
This project analyzes credit card transaction data using SQL and pandas to identify key fraud patterns, assess risk levels, and support fraud prevention strategies. The analysis aims to highlight when, where, and how fraudulent activity tends to occur empowering more informed risk segmentation and detection modeling.
## Problem Statement
Credit card fraud poses serious challenges for financial institutions, requiring robust, data-driven strategies to detect and prevent suspicious activity.
The goal of this project is to explore transaction-level data to uncover meaningful insights that distinguish fraudulent from legitimate transactions.
## Dataset
Due to file size limits, access the dataset from the link below:  
Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
Source: Kaggle Credit Card Fraud Detection Dataset
Rows: 284,807 transactions
Class Labels: 1 = fraud, 0 = non-fraud
Amount: Transaction value in euros
Time: Seconds elapsed since the first transaction
## Tools & Skills Used
SQL (SQLite) via pandas.read_sql
pandas for analysis
Python (Jupyter Notebook)
Analytical Thinking & Feature Engineering
## Key Analyses Performed
1. Risk Segmentation Analysis
Created a custom risk score based on transaction amount and time of day
Segmented transactions into: Minimal, Low, Medium, and High Risk
Evaluated fraud rate, average amount, and total loss for each category
2. Time-of-Day Fraud Patterns
Grouped transactions into 4-hour blocks (e.g., “Late Night”, “Morning”)
Found that fraud rates are higher during late-night and early-morning hours
Compared fraud volume and average transaction size across time blocks
3. Transaction Value Bucketing
Binned transaction amounts into ranges (e.g. $0–25, $500–1000, $2000+)
Measured fraud prevalence per range
Found higher fraud concentration in $0–25 and $2000+ buckets
4. Business Impact Summary
Quantified overall fraud loss vs. high-value fraud loss
Showed how a small portion of transactions contribute disproportionately to losses
## Key Insights
1. Fraud occurs disproportionately late at night (12am–6am)
2. High-value transactions (>$1000) contribute a large share of total fraud loss
3. Low-amount transactions are also frequent targets for fraud
4. Custom risk scores can help pre-flag suspicious transactions for review

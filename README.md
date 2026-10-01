# Telco Customer Churn Analysis

## Overview
An end-to-end data analysis project exploring customer churn for a telecom 
company, using Python for data cleaning and EDA, SQL for business-focused 
querying, and Power BI for an interactive dashboard. The goal: identify why 
customers churn and recommend retention strategies.

## Business Problem
Customer churn costs telecom companies significant recurring revenue. This 
project analyzes 7,032 customer records to answer:
- What is the overall churn rate?
- Which customer segments are most at risk?
- What retention strategies would have the biggest impact?

## Tools Used
- **Python** (pandas, matplotlib, seaborn) — data cleaning & EDA
- **SQL** (SQLite) — business queries
- **Power BI** — interactive dashboard

## Dataset
IBM Telco Customer Churn dataset (Kaggle) — 7,043 customers, 21 attributes 
including demographics, account info, services subscribed, and churn status.

## Process
1. **Data Cleaning**: Fixed data types, handled 11 missing values in 
   TotalCharges, verified no duplicates
2. **EDA**: Analyzed churn patterns across contract type, tenure, payment 
   method, internet service, and monthly charges
3. **SQL Analysis**: Queried churn rate by segment and revenue at risk
4. **Dashboard**: Built an interactive Power BI dashboard with KPI cards, 
   segment breakdowns, and filters

## Key Insights
- **Overall churn rate: 26.58%**, representing **$139.13K/month** in lost 
  revenue
- **Contract type is the strongest churn driver** — month-to-month customers 
  churn far more than annual contract holders
- **Electronic check payers churn at 45.3%**, nearly 3x higher than 
  automatic payment methods
- **New customers (0–12 months tenure) are highest risk** — churn drops 
  sharply after the first year
- **Fiber optic customers churn more than DSL customers**, suggesting a 
  pricing or service satisfaction issue
- Churned customers pay **higher average monthly bills** than retained ones

## Recommendations
1. Incentivize month-to-month customers to switch to annual contracts
2. Encourage migration from electronic check to autopay
3. Build a stronger first-year onboarding and retention program
4. Investigate fiber optic service pricing and satisfaction

## Files
- `Untitled1.ipynb` — full Python cleaning & EDA
- `telco_churn_cleaned.csv` — cleaned dataset

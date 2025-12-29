```markdown
# Customer Shopping Behavior — Full Project README

_Industry-style end-to-end analysis of retail customer transactions with SQL, Python, and Power BI._

---

## Table of Contents
- Overview
- Business Problem
- Dataset
- Tools & Technologies
- Project Structure
- Data Cleaning & Transformation
- Key Analyses
- SQL Queries
- Dashboard
- How to run
- Deliverables
- Recommendations
- Author & Contact

---

## Overview

This portfolio project demonstrates an end-to-end analytics workflow: cleaning raw transactions, generating business metrics in SQL, exploring customer segments in Python, and building a Power BI dashboard for stakeholders.

## Business Problem

- Identify who the best customers are and how to retain them.
- Understand seasonal and category-level demand patterns.
- Measure promotion effectiveness and recommend targeting strategies.

## Dataset

- File: `customer_shopping_behavior.csv`
- Key fields: `Customer ID`, `Age`, `Gender`, `Item Purchased`, `Category`, `Purchase Amount (USD)`, `Season`, `Review Rating`, `Subscription Status`, `Promo Code Used`, `Previous Purchases`, `Payment Method`, `Frequency of Purchases`.

## Tools & Technologies

- Python: pandas, numpy, matplotlib, seaborn
- SQL: example queries included for analytics
- Power BI: interactive dashboard file included (if present)

## Project Structure

```
customer-trends-data-analysis-SQL-Python-PowerBI/
├── Customer_Shopping_Behavior_Analysis.ipynb
├── customer_shopping_behavior.csv
├── customer_behavior_sql_queries.sql
├── customer_behavior_dashboard.pbix
├── README_FULL.md
└── images/ (exported visuals)
```

## Data Cleaning & Transformation

- Standardized category names and payment methods.
- Imputed or removed invalid/missing values for key metrics (Purchase Amount, Season).
- Engineered `LTV`-style aggregates and cohort labels for retention analysis.

## Key Analyses

- RFM-style customer segmentation to identify top revenue contributors.
- Seasonal demand analysis by category to guide promotional timing.
- Promotion lift analysis comparing AOV and repeat rate between promo and non-promo cohorts.

## SQL Queries

- See `customer_behavior_sql_queries.sql` for repeatable metrics: cohort tables, retention queries, and lifetime value calculations.

## Dashboard

- Open `customer_behavior_dashboard.pbix` in Power BI to interact with cohort, retention, and revenue visuals.

## How to run

1. Create Python environment and install dependencies:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install pandas matplotlib seaborn sqlalchemy jupyter nbconvert
```

2. Run the notebook and export HTML:

```powershell
jupyter nbconvert --to html Customer_Shopping_Behavior_Analysis.ipynb --output CustomerShopping_report.html
```

## Deliverables

- Cleaned dataset and cohort tables
- Notebook with EDA and visuals
- SQL query file for reproducible metrics
- Power BI dashboard (interactive)

## Recommendations (high-level)

- Prioritize retention programs for the top 10% of customers by revenue.
- Target seasonal promotions for high-conversion categories.
- Monitor promo profitability per cohort to avoid margin erosion.

---

## Author & Contact

**Khush Agrawal**  
LinkedIn: <YOUR_LINKEDIN_URL>  
GitHub: <YOUR_GITHUB_URL>  
Portfolio / Codolio: <YOUR_CODOLIO_URL>

```

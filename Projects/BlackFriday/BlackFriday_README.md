# Black Friday Retail Analytics  
### End-to-End Exploratory Data Analysis & Feature Engineering for Purchase Prediction

**Author:** Khush Agrawal  
🔗 LinkedIn: https://www.linkedin.com/in/khush-agrawal007  
🔗 GitHub: https://github.com/Khush-Agrawal-007  
🔗 Portfolio: https://codolio.com/profile/khushagrawal  

---

## 1. Project Overview

This project performs **end-to-end exploratory data analysis (EDA) and feature engineering** on a Black Friday retail transactions dataset to prepare it for **predictive modeling and business decision-making**.

The focus is on transforming raw, messy transactional data into a **clean, structured, and model-ready dataset**, while extracting insights about customer behavior and product performance.

A reviewer should be able to understand the **entire problem, approach, and outcome by reading this README alone**.

---

## 2. Business Problem & Motivation

Retail businesses struggle to identify:
- High-value customers
- High-performing product categories
- Patterns that drive purchase value during large-scale sales events

This project addresses those challenges by analyzing historical Black Friday transactions and engineering features that can be used to **predict purchase amount**, **segment customers**, or **optimize marketing strategies**.

---

## 3. Dataset Description

- **Source:** Black Friday retail transactions dataset (Kaggle-style dataset)
- **Records:** ~[Number of rows]
- **Features:** User demographics, product categories, and purchase amount

### Key Columns
- `User_ID` – Unique customer identifier  
- `Product_ID` – Unique product identifier  
- `Gender`, `Age`, `Occupation` – Customer demographics  
- `City_Category`, `Stay_In_Current_City_Years` – Location-related indicators  
- `Product_Category_1`, `Product_Category_2`, `Product_Category_3` – Product hierarchy  
- `Purchase` – Target variable (transaction amount)

---

## 4. Project Pipeline

1. Data ingestion and initial inspection  
2. Missing value analysis and treatment  
3. Data type correction and consistency checks  
4. Exploratory Data Analysis (EDA)  
5. Feature engineering (user-level and product-level)  
6. Validation of model readiness  

All steps are implemented and documented in the Jupyter Notebook.

---

## 5. Data Cleaning & Preprocessing

Key data issues addressed:
- High missing values in `Product_Category_2` and `Product_Category_3`
- Categorical variables stored as numeric codes
- Skewed distribution of the `Purchase` variable

Cleaning actions:
- Logical imputation for missing categorical features
- Standardized categorical representations
- Validation of feature ranges and consistency

---

## 6. Exploratory Data Analysis (EDA)

EDA was conducted to extract **business-relevant insights**, including:
- Distribution and skewness of purchase amounts
- Spending patterns across gender and age groups
- Revenue contribution by product categories
- Relationship between purchase frequency and average spend

These insights help identify **customer segments** and **high-impact product categories**.

---

## 7. Feature Engineering

Feature engineering is the core strength of this project.

### Engineered Features
- **User-level features**
  - Total purchase count per user
  - Average purchase value
  - Purchase frequency indicators

- **Product-level features**
  - Product popularity metrics
  - Category-level aggregation features

- **Encoded categorical variables**
  - Prepared for both linear and tree-based models

These features significantly improve the dataset’s suitability for machine learning.

---

## 8. Model Readiness & Next Steps

The cleaned and feature-engineered dataset is ready for:
- Regression models to predict `Purchase`
- Customer segmentation
- Recommendation systems

Suggested models:
- Linear Regression (baseline)
- Random Forest
- Gradient Boosting / XGBoost

---

## 9. Deliverables

- Jupyter Notebook containing:
  - Data cleaning
  - EDA
  - Feature engineering
- Cleaned, feature-engineered dataset (exported from the notebook)
- Reproducible analysis workflow

---

## 10. How to Run the Project

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install pandas numpy scikit-learn matplotlib seaborn jupyter nbconvert
jupyter nbconvert --to html "2- BlackFriday EDA And Feature Engineering.ipynb" --output BlackFriday_Report.html

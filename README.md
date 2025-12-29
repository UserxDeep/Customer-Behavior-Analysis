# 🛍️ Customer Shopping Behavior Analysis

An end-to-end data analytics project analyzing customer shopping behavior using Python, SQL, and Power BI.  
The project focuses on uncovering spending patterns, customer segments, product performance, and subscription behavior to support data-driven business decisions.

---

## 📌 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Tools & Technologies](#tools--technologies)
- [Project Workflow](#project-workflow)
- [SQL Analysis](#sql-analysis)
- [Dashboard](#dashboard)
- [Key Insights](#key-insights)
- [Business Recommendations](#business-recommendations)

---

## Overview
This project analyzes **3,900 customer transactions** across multiple product categories to understand how customers shop, spend, and respond to discounts and subscriptions.

The analysis covers:
- Customer demographics
- Purchase behavior
- Product performance
- Subscription and loyalty trends

---

## Dataset
- **Rows:** 3,900  
- **Columns:** 18  
- **Data Type:** Transactional retail data  

### Key Features
- **Customer Info:** Age, Gender, Location, Subscription Status  
- **Purchase Details:** Item Purchased, Category, Amount, Season, Size, Color  
- **Behavioral Data:** Discounts, Promo Codes, Previous Purchases, Review Ratings, Shipping Type  

<details>
<summary>📄 Data Quality Notes</summary>

- 37 missing values found in the `review_rating` column  
- Missing ratings were imputed using the **median rating per product category**  
- Redundant column `promo_code_used` was removed  

</details>

---

## Tools & Technologies
- 🐍 **Python** – Pandas, NumPy (EDA & Data Cleaning)
- 🗄️ **SQL** – PostgreSQL (Business Analysis Queries)
- 📊 **Power BI** – Interactive Dashboard
- 📓 **Jupyter Notebook** – Analysis & Documentation

---

## Project Workflow
1. **Data Loading**
   - Imported dataset using Pandas
   - Verified structure and data types

2. **Exploratory Data Analysis (EDA)**
   - Summary statistics and distributions
   - Identified missing values and inconsistencies

3. **Data Cleaning & Feature Engineering**
   - Imputed missing review ratings
   - Standardized column names (snake_case)
   - Created:
     - `age_group`
     - `purchase_frequency_days`
   - Removed redundant columns

4. **Database Integration**
   - Loaded cleaned data into PostgreSQL
   - Performed structured SQL analysis

---

## SQL Analysis
Key business questions answered using SQL:

1. **Revenue by Gender**
2. **High-Spending Discount Users**
3. **Top 5 Products by Average Rating**
4. **Shipping Type Comparison (Standard vs Express)**
5. **Subscribers vs Non-Subscribers Spend**
6. **Discount-Dependent Products**
7. **Customer Segmentation (New, Returning, Loyal)**
8. **Top 3 Products per Category**
9. **Repeat Buyers & Subscription Likelihood**
10. **Revenue Contribution by Age Group**

<details>
<summary>📊 Sample Findings</summary>

- Male customers generated higher total revenue than female customers  
- Express shipping users spent slightly more on average  
- Subscribers contributed significantly higher total revenue  
- Loyal customers formed the largest customer segment  

</details>

---

## Dashboard
An interactive **Power BI dashboard** was created to visualize:
- KPIs (Average Purchase Amount, Ratings, Customer Count)
- Revenue by category and age group
- Subscription and shipping behavior
- Customer segmentation

📷 *Dashboard preview can be added here as an image if desired.*

---

## Key Insights
- Customers using discounts can still be high spenders
- A small group of products drives a large share of revenue
- Loyal customers dominate the customer base
- Certain age groups contribute more consistently to revenue
- Subscription status strongly correlates with total spend

---

## Business Recommendations
- **Boost Subscriptions:** Promote exclusive subscriber benefits  
- **Customer Loyalty Programs:** Reward repeat buyers to build loyalty  
- **Discount Strategy:** Balance discounts with margin control  
- **Product Positioning:** Highlight top-rated and best-selling products  
- **Targeted Marketing:** Focus campaigns on high-revenue age groups and express-shipping users  

---

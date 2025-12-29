# Customer Shopping Behavior Analysis 🛍️

## 📊 Overview
[cite_start]This project analyzes transactional data from **3,900 purchases** to uncover deep insights into customer spending patterns, segmentation, and product preferences[cite: 3]. [cite_start]By leveraging **Python** for data engineering, **SQL** for business logic, and **Power BI** for visualization, this analysis provides data-driven recommendations to optimize subscription behavior and strategic business growth[cite: 4, 115].

---

## 📂 Dataset Summary
* [cite_start]**Scale:** 3,900 rows and 18 columns[cite: 6].
* [cite_start]**Demographics:** Age, Gender, Location, and Subscription Status[cite: 8].
* [cite_start]**Transaction Details:** Item Purchased, Category, Purchase Amount, Season, and Size[cite: 9].
* [cite_start]**Behavioral Metrics:** Discount Usage, Previous Purchases, Review Ratings, and Shipping Type[cite: 10].
* [cite_start]**Data Quality:** Handled 37 missing values in the `Review Rating` column[cite: 11].

---

## 🛠️ Tools & Technologies
* [cite_start]**Python (Pandas):** Data cleaning, missing value imputation, and feature engineering[cite: 13, 14, 23].
* [cite_start]**PostgreSQL:** Advanced querying for revenue analysis and customer segmentation[cite: 27, 29].
* [cite_start]**Power BI:** Interactive dashboarding and KPI tracking[cite: 115].

---

## 🚀 Project Steps

### 1. Data Cleaning & EDA (Python)
* [cite_start]**Standardization:** Renamed columns to snake_case and converted data types[cite: 21].
* [cite_start]**Missing Data:** Imputed `Review Rating` nulls using the median rating per product category[cite: 20].
* [cite_start]**Feature Engineering:** Binned ages into groups and created a `purchase_frequency_days` column[cite: 24, 25].
* [cite_start]**Consistency:** Dropped redundant columns like `promo_code_used` after verifying overlap with `discount_applied`[cite: 26].

### 2. Structured SQL Analysis
[cite_start]I loaded the cleaned data into PostgreSQL to answer critical business questions[cite: 27, 29]:
* [cite_start]**Revenue Drivers:** Compared Male ($157,890) vs. Female ($75,191) total revenue[cite: 30, 36, 39].
* [cite_start]**Customer Segmentation:** Classified users into **Loyal** (3,116), **Returning** (701), and **New** (83) segments[cite: 91].
* [cite_start]**Product Performance:** Identified the top-rated products (Gloves, Sandals, Boots) and high-volume items per category (Jewelry, Blouses, Jackets)[cite: 81, 93].
* [cite_start]**Subscription Impact:** Found that while subscribers have a slightly lower average spend ($59.49) than non-subscribers ($59.87), they represent a key loyalist base[cite: 86].

### 3. Power BI Dashboarding
[cite_start]Developed an interactive dashboard to visualize[cite: 115]:
* [cite_start]**High-Level KPIs:** Total Customers (3.9K), Average Purchase ($59.76), and Average Rating (3.75)[cite: 120, 122, 124].
* [cite_start]**Sales Trends:** Breakdown of revenue by category (Clothing being the leader) and Age Group[cite: 129, 145].
* [cite_start]**Filterable Insights:** Users can slice data by Gender, Subscription Status, and Shipping Type[cite: 125, 116, 138].

---

## 🏆 Key Results & Recommendations
* [cite_start]**Demographic Focus:** Focus marketing on the **Young Adult** group, which generates the highest revenue ($62,143)[cite: 103, 104].
* [cite_start]**Loyalty Programs:** Reward the 3,116 "Loyal" customers to maintain retention and move "Returning" customers into the loyal tier[cite: 91, 157].
* [cite_start]**Shipping Optimization:** Express-shipping users show higher average spend; consider offering it as a perk for the "Returning" segment to boost sales[cite: 83, 160].
* [cite_start]**Subscription Growth:** Only 27% of customers are currently subscribers [cite: 132][cite_start]; promote exclusive benefits to convert the 73% non-subscriber base[cite: 144, 153].

---

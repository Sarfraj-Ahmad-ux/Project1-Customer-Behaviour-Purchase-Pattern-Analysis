# Customer Behavior & Purchase Pattern Analysis

## Table of Contents
- [1. Project Title](#1-project-title)
- [2. Brief One Line Summary](#2-brief-one-line-summary)
- [3. Overview](#3-overview)
- [4. Problem Statement](#4-problem-statement)
- [5. Data Sets](#5-data-sets)
- [6. Tools And Technologies](#6-tools-and-technologies)
- [7. Methods](#7-methods)
- [8. Key Insights](#8-key-insights)
- [9. Dashboard](#9-dashboard)
- [10. Result And Conclusion](#10-result-and-conclusion)

---

## 1. Project Title
**Customer Behavior & Purchase Pattern Analysis**

---

## 2. Brief One Line Summary
An end-to-end data analytics project processing retail transactional data in Python, querying business metrics using MySQL, and building interactive Power BI dashboards to drive revenue growth[cite: 3].

---

## 3. Overview
This project synthesizes raw retail transactional data into actionable business intelligence[cite: 3]. It covers data cleaning and feature binning in Python, relational database modeling and analytical querying in MySQL Workbench, and interactive visualization in Power BI to evaluate revenue drivers, product performance, and customer retention metrics[cite: 3].

---

## 4. Problem Statement
Retail businesses often struggle to identify key revenue drivers, assess discount reliance, and convert single-time buyers into loyal subscribers[cite: 3]. This project aims to analyze 3,900 customer transactions to uncover purchasing habits, evaluate category-level performance, and provide data-backed strategies to optimize subscriber conversion and basket values[cite: 3].

---

## 5. Data Sets
- **Dataset Size:** 3,900 transactional records (~4K records) across 4,000 unique customers[cite: 3].
- **Attributes Analyzed:** Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount ($), Location, Size, Color, Season, Review Rating, Subscription Status, Shipping Type, Discount Applied, and Previous Purchases[cite: 3].

---

## 6. Tools And Technologies
- **Data Preprocessing:** Python (Jupyter Notebook - `Project1.ipynb`, Pandas)[cite: 3]
- **Database Management & SQL Querying:** MySQL Workbench (`PROJECT1` Database)[cite: 3]
- **Data Visualization & BI Dashboards:** Power BI Desktop[cite: 3]

---

## 7. Methods
1. **Data Sanitization & Preprocessing (Python):**
   - Imputed missing values across review ratings, shipping options, and discounts[cite: 3].
   - Standardized column headers into clean `snake_case` format (e.g., `purchase_amount`, `review_rating`)[cite: 3].
   - Binned customer ages into demographic groups (`Young Adult`, `Adult`, `Middle Aged`, `Senior`)[cite: 3].
   - Cast purchase volumes and binary flags into uniform data types[cite: 3].

2. **Database Querying & Analysis (MySQL):**
   - Calculated revenue share by gender, fulfillment type, and age demographic[cite: 3].
   - Applied aggregate & window functions (`PARTITION BY`) to rank top-selling products per category[cite: 3].
   - Analyzed discount usage vs. baseline spend to flag high-value discount-sensitive buyers[cite: 3].
   - Segmented customer cohorts into `New`, `Returning`, and `Loyal` based on order history[cite: 3].

3. **Dashboard Design (Power BI):**
   - Built interactive slicers (Category, Gender, Discount Applied, Age Group).
   - Structured visual KPI cards for Total Quantity (233K), Unique Customers (4K), and Avg Purchase Quantity (59.76)[cite: 3].
   - Designed custom charts for Sales by Location, Category Performance, Subscription Breakdown, and Product Ratings.

---

## 8. Key Insights
- **Category Performance:** **Clothing** is the top-performing category generating **104K** in sales volume across **3.40M** interactions, followed by **Accessories (74K)** and **Footwear (36K)**[cite: 3].
- **Subscription Gap:** Non-subscribers account for **73.12% ($170K)** of total sales volume, whereas subscribers generate only **26.88% ($63K)**[cite: 3].
- **Discount Sensitivity:** High-value customers frequently use discounts while maintaining basket sizes above the baseline average of **59.76**[cite: 3].
- **Top Product Ratings:** Product satisfaction remains strong overall, led by **Gloves (3.86/5)**, **Sandals (3.84/5)**, **Boots (3.82/5)**, **Hat (3.80/5)**, and **Skirt (3.78/5)**[cite: 3].

---

## 9. Dashboard
Below is the interactive Power BI Customer Behavior Dashboard developed for this analysis:

![Customer Behavior Dashboard](./dashboard.png)

*(Note: Save your uploaded dashboard image as `dashboard.png` inside the same GitHub repository folder so it renders automatically on GitHub)*

---

## 10. Result And Conclusion
1. **Subscription Conversion Strategy:** Focus acquisition efforts on converting the **73.12% non-subscriber majority**, specifically targeting repeat buyers (>5 previous purchases) with loyalty perks[cite: 3].
2. **Category Prioritization:** Double down on hero placement and inventory allocation for **Clothing** and **Accessories**, which account for over 76% of total revenue[cite: 3].
3. **Threshold Promotions:** Shift discount strategies for high-spending buyers from flat discounts to minimum spend thresholds (e.g., *"Get $10 off on orders over $75"*) to raise average order values past **$59.76**[cite: 3].
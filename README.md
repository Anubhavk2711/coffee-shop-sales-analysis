<img width="987" height="596" alt="image" src="https://github.com/user-attachments/assets/058633fa-5077-4bc9-bdcb-096a0f0958ad" /># ☕ Coffee Shop Sales Analysis (SQL + Power BI)

## 📌 Project Overview

This project focuses on analyzing coffee shop sales data using **MySQL** and visualizing insights using **Power BI**. The goal is to solve real-world business problems by extracting meaningful insights from raw data.

---

## 🎯 Objectives

* Analyze **monthly sales trends**
* Identify **month-on-month growth**
* Track **total orders and quantity sold**
* Find **top-performing products**
* Analyze **sales patterns by day, hour, and location**

---

## 🧠 Problem Statement

The project answers key business questions:

### 1. Sales Analysis

* Total sales per month
* Month-on-month increase/decrease
* Difference between current and previous month

### 2. Orders Analysis

* Total orders per month
* MoM change in orders

### 3. Quantity Sold Analysis

* Total quantity sold per month
* MoM trends

📊 *(Based on project slides — see pages 7–9)* 

---

## 🛠️ Tech Stack

* **MySQL** – Data cleaning & analysis
* **Power BI** – Dashboard & visualization
* **Excel/CSV** – Raw dataset

---

## ⚙️ Workflow

### 🔹 Step 1: Data Preparation

* Imported raw dataset into MySQL
* Cleaned and formatted data
* Changed data types

### 🔹 Step 2: SQL Analysis

Used SQL queries to:

* Calculate total sales
* Perform time-based analysis (Month, Day, Hour)
* Use window functions (LAG, etc.)

Example:

```sql
SELECT 
    MONTH(transaction_date) AS month,
    SUM(unit_price * transaction_qty) AS total_sales
FROM coffee_shop_sales
GROUP BY MONTH(transaction_date);
```

📌 *(Refer page 2 for SQL logic)* 

---

### 🔹 Step 3: Power BI Dashboard

Created interactive dashboard with:

* Calendar Heat Map
* Sales by Weekdays vs Weekends
* Store-wise Sales
* Daily Sales with Average Line
* Top 10 Products
* Sales by Hours

📊 *(Dashboard requirements from pages 8–9)* 

---

## 📊 Key Insights

* Identified peak sales months
* Found best-selling products
* Discovered hourly sales trends
* Compared weekday vs weekend performance

---

## 📸 Dashboard Preview

<img width="987" height="596" alt="image" src="https://github.com/user-attachments/assets/e4865ab7-bb6c-44fc-a231-d63340ce38f4" />



---

## 📂 Project Files

* `data/` → Raw dataset
* `sql/` → SQL queries
* `dashboard/` → Power BI file
* `images/` → Dashboard screenshots

---

## 🚀 How to Run

1. Import dataset into MySQL
2. Run SQL queries from `/sql`
3. Open `.pbix` file in Power BI
4. Connect dataset and refresh

---

## 📚 Learnings

* SQL window functions (LAG, GROUP BY)
* Data cleaning & transformation
* Data visualization best practices
* Business KPI analysis

---

## 🤝 Connect

If you like this project, feel free to ⭐ the repo!

---

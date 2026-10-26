# 🛒 Retail & E-Commerce Sales Analytics (MySQL)

## 📌 Project Overview
This repository contains an end-to-end relational database analysis for a retail and e-commerce business. The project demonstrates practical SQL querying capabilities, ranging from transactional schema architecture and data cleaning to complex multi-table joins, Common Table Expressions (CTEs), and advanced window functions to solve real-world business intelligence scenarios.

---

## 🗄️ Database Architecture & Schema
The relational structure centers around three normalized tables:
- **`customers`**: Customer demographic profiles, locations (cities/states), and registration metadata.
- **`products`**: Product catalog details, unit pricing, categories, and inventory classifications.
- **`orders`**: Transactional records capturing order quantities, dates, payment methods (UPI, Credit Card, Net Banking), and fulfillment statuses.

---

## 🚀 Key SQL Concepts Demonstrated

### 1. Multi-Table Relational Joins
- Merged transactional records across `customers`, `products`, and `orders` using `INNER JOIN` and `LEFT JOIN`.
- Aggregated gross and net revenues across geographic territories, product lines, and payment gateways.

### 2. Advanced Window Functions
- **`ROW_NUMBER()` & `DENSE_RANK()`**: Ranked top revenue-generating products and segmented high-value customer tiers within individual cities.
- **`SUM() OVER (PARTITION BY ... ORDER BY ...)`**: Computed cumulative running revenue totals across order timelines.
- **`LAG()` & `LEAD()`**: Evaluated order-over-order sales variances and tracked period-over-period performance swings.

### 3. Common Table Expressions (CTEs) & Subqueries
- Structured complex analytical pipelines using modular CTEs (`WITH` clauses) for readability and performance.
- Implemented nested subqueries and conditional `HAVING` filters to identify underperforming inventories and inactive accounts.

### 4. Scenario-Based Business Analysis
- Solved 20+ realistic operational business challenges including managerial self-joins, departmental salary distributions, and login session durations using time-difference transformations (`TIMEDIFF`).

---

## 📂 Repository Contents
- **`A KISHOR 28th sept SQL_Final_EXAM.sql`**: Comprehensive script containing table DDL/DML, multi-table aggregations, CTEs, and advanced window function implementations.
- **`20QUESmysqlscenariobasedsqlquestionsdocx-21SEP.docx`**: Detailed business scenarios, relational challenge descriptions, and analytical problem statements.

---

## 🛠️ Tools & Technologies
- **Database Engine:** MySQL / Relational Database Management System (RDBMS)
- **Concepts:** Multi-Table Joins, Window Functions, CTEs, Subqueries, Aggregations, Date-Time Functions

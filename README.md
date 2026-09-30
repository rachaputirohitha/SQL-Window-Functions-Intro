# Task 23 – SQL Window Functions Intro

## Project Overview

This project demonstrates the use of SQL Window Functions to solve practical business questions using the Northwind database.

The task was completed using MySQL Workbench and covers:

- ROW_NUMBER()
- RANK()
- DENSE_RANK()
- LAG()
- PARTITION BY
- GROUP BY
- CTEs
- Date and order-value comparisons

## Dataset

The project uses the Northwind sample database.

### Dataset Validation

| Table | Records |
|---|---:|
| Customers | 29 |
| Products | 45 |
| Orders | 48 |
| Order Details | 58 |

## Tools Used

- MySQL
- MySQL Workbench
- Northwind Dataset

## SQL Concepts Covered

### 1. ROW_NUMBER()

Used to assign sequential numbers to orders and to identify the latest order for each customer.

### 2. RANK()

Used to rank products by price and customers by number of orders.

### 3. DENSE_RANK()

Used together with RANK() to understand how ranking behaves when values are tied.

### 4. PARTITION BY

Used to perform window calculations separately for each customer or product category.

### 5. LAG()

Used to access previous order dates and previous order amounts.

### 6. Business Analysis

The queries were used to answer questions such as:

- What is the sequence of orders?
- What is each customer's order number?
- What is the latest order for each customer?
- Which products have the highest prices?
- Which customers have the most orders?
- How are products ranked within categories?
- How many days have passed since a customer's previous order?
- How has the current order amount changed compared with the previous order?

## Queries Completed

A total of 12 SQL queries were completed.

1. Number orders chronologically using ROW_NUMBER()
2. Number orders separately for each customer
3. Find the latest order for each customer
4. Rank products by list price
5. Rank customers by number of orders
6. Rank products within each category
7. Compare RANK() and DENSE_RANK()
8. Find the previous order date using LAG()
9. Calculate days since the previous order
10. Compare current and previous order amounts
11. Compare each customer's current and previous order
12. Classify order trends as First Order, Increased, Decreased, or No Change

## Key Learnings

- Window functions allow calculations across related rows without losing individual row details.
- ROW_NUMBER() is useful for sequential numbering.
- RANK() and DENSE_RANK() are useful for ranking and handling ties.
- LAG() is useful for comparing a row with a previous row.
- PARTITION BY allows window calculations to restart for each group.
- CTEs can make complex SQL analysis easier to understand.

## Conclusion

This task provided practical experience with SQL Window Functions and demonstrated how they can be used to perform ranking, sequencing, previous-value comparisons, and business trend analysis on relational data.

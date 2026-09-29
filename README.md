# E-Commerce Customer Churn Analysis

## Project Overview

This project analyzes customer churn in an e-commerce dataset using **MySQL and SQL**. The project covers data cleaning, data transformation, exploratory data analysis, and customer behavior analysis.

The analysis focuses on factors such as **churn, tenure, payment methods, order categories, coupon usage, satisfaction, complaints, cashback, and warehouse distance**.

## Objectives

* Clean and prepare the customer churn dataset
* Handle missing values
* Identify and remove outliers
* Standardize inconsistent data
* Create derived fields for analysis
* Compare churned and active customers
* Analyze customer behavior across different segments
* Use SQL for data analysis and business insights
* Demonstrate relational database concepts using JOINs

## Tools & Technologies

* **MySQL**
* **SQL**
* **MySQL Workbench**

## Project Files

### `customer_churn_db.sql`

Contains the database and table creation along with the original dataset.

### `Customerchurn_Datacleaning.sql`

Contains queries for:

* Missing value analysis
* Mean and mode imputation
* Outlier identification and removal
* Data standardization
* Column renaming
* Data transformation

### `Customer_churn_analysis.sql`

Contains queries for:

* Churn analysis
* Customer segmentation
* Payment method analysis
* Order category analysis
* Coupon and cashback analysis
* Satisfaction and complaint analysis
* Warehouse distance analysis
* Subqueries
* Customer return analysis using JOINs

## Data Cleaning & Transformation

The dataset was prepared using SQL by:

* Handling missing values using mean and mode imputation
* Removing warehouse distance outliers
* Standardizing categorical values
* Renaming columns for better readability
* Creating `ComplaintReceived` to represent complaint status
* Creating `ChurnStatus` to identify active and churned customers
* Creating warehouse distance categories

### Warehouse Distance Categories

| Distance | Category   |
| -------- | ---------- |
| ≤ 5      | Very Close |
| 6–10     | Close      |
| 11–15    | Moderate   |
| > 15     | Far        |

## Analysis Performed

The project analyzes:

* Churned and active customer counts
* Average tenure of churned customers
* Customer complaints and churn
* Churn by city tier and order category
* Preferred payment methods
* Coupon usage
* Cashback by order category
* Customer satisfaction
* Order behavior
* Warehouse distance and churn
* Customer segments using subqueries
* Customer returns using relational JOINs

## Customer Returns Analysis

A separate `Customer_returns` table was created to demonstrate relational database concepts.

The table contains:

* `ReturnID`
* `CustomerID`
* `ReturnDate`
* `RefundAmount`

A foreign key relationship was created between `Customer_returns` and the customer churn table using `CustomerID`.

An `INNER JOIN` was used to analyze return details for relevant customers.

## SQL Concepts Used

* SELECT
* WHERE
* GROUP BY
* ORDER BY
* LIMIT
* COUNT()
* SUM()
* AVG()
* MAX()
* CASE
* HAVING
* Subqueries
* INNER JOIN
* Primary Keys
* Foreign Keys
* ALTER TABLE
* UPDATE
* DELETE

## Key Learning Outcomes

This project helped me gain practical experience in:

* SQL data cleaning
* Data transformation
* Exploratory data analysis
* Customer churn analysis
* Aggregate functions
* Subqueries
* CASE statements
* GROUP BY and HAVING
* Relational database concepts
* SQL JOINs

## Author

**Hanna**

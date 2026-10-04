# pr2sql
# 📊 SQL Data Transformation Project

> **A practical SQL project demonstrating JOINs, Subqueries, Date Functions, String Functions, Window Functions, and CASE Statements using MySQL/MariaDB.**

---

## 🌟 Project Overview

This project is designed to demonstrate important **SQL data transformation and analysis techniques** using **XAMPP/phpMyAdmin (MySQL/MariaDB)**.

The project works with three main tables:

* 👤 **Customers**
* 🛒 **Orders**
* 👨‍💼 **Employees**

It contains **17 practical SQL queries** covering different concepts used in real-world database applications.

---

## 🎯 Objectives

The main objectives of this project are:

* Understand different types of **SQL JOINs**
* Work with **subqueries**
* Use **date and time functions**
* Perform **string manipulation**
* Calculate **running totals**
* Rank records using **window functions**
* Apply conditional logic using **CASE**
* Analyze customer orders and employee salaries
* Practice SQL using **XAMPP/phpMyAdmin**

---

## 🛠️ Technologies Used

| Technology         | Purpose                 |
| ------------------ | ----------------------- |
| 🐬 MySQL / MariaDB | Database                |
| 🖥️ XAMPP          | Local Server            |
| 🌐 phpMyAdmin      | Database Management     |
| 💻 SQL             | Queries & Data Analysis |

---

# 🗄️ Database Structure

## 👤 Customers

| Column           | Data Type | Description         |
| ---------------- | --------- | ------------------- |
| CustomerID       | INT       | Unique Customer ID  |
| FirstName        | VARCHAR   | Customer first name |
| LastName         | VARCHAR   | Customer last name  |
| Email            | VARCHAR   | Customer email      |
| RegistrationDate | DATE      | Registration date   |

### Sample Data

| ID | First Name | Last Name | Email                                               | Registration Date |
| -: | ---------- | --------- | --------------------------------------------------- | ----------------- |
|  1 | John       | Doe       | [john.doe@email.com](mailto:john.doe@email.com)     | 2022-03-15        |
|  2 | Jane       | Smith     | [jane.smith@email.com](mailto:jane.smith@email.com) | 2021-11-02        |

---

## 🛒 Orders

| Column      | Data Type | Description        |
| ----------- | --------- | ------------------ |
| OrderID     | INT       | Unique Order ID    |
| CustomerID  | INT       | Customer reference |
| OrderDate   | DATE      | Date of order      |
| TotalAmount | DECIMAL   | Total order amount |

### Sample Data

| Order ID | Customer ID | Order Date | Total Amount |
| -------: | ----------: | ---------- | -----------: |
|      101 |           1 | 2023-07-01 |       150.50 |
|      102 |           2 | 2023-07-03 |       200.75 |

---

## 👨‍💼 Employees

| Column     | Data Type | Description         |
| ---------- | --------- | ------------------- |
| EmployeeID | INT       | Unique Employee ID  |
| FirstName  | VARCHAR   | Employee first name |
| LastName   | VARCHAR   | Employee last name  |
| Department | VARCHAR   | Employee department |
| HireDate   | DATE      | Hiring date         |
| Salary     | DECIMAL   | Employee salary     |

### Sample Data

| ID | First Name | Last Name | Department | Hire Date  |   Salary |
| -: | ---------- | --------- | ---------- | ---------- | -------: |
|  1 | Mark       | Johnson   | Sales      | 2020-01-15 | 50000.00 |
|  2 | Susan      | Lee       | HR         | 2021-03-20 | 55000.00 |

---

# 📚 SQL Concepts Covered

### 🔗 1. JOIN Operations

The project demonstrates:

* `INNER JOIN`
* `LEFT JOIN`
* `RIGHT JOIN`
* `FULL OUTER JOIN` concept using `UNION`

> 💡 **Note:** MySQL/MariaDB does not directly support `FULL OUTER JOIN`, so a combination of `LEFT JOIN`, `RIGHT JOIN`, and `UNION` is used.

---

### 🔍 2. Subqueries

Subqueries are used to find:

* Customers whose orders are **above the average order amount**
* Employees whose salaries are **above the average salary**

---

### 📅 3. Date Functions

The project uses:

```sql
YEAR()
MONTH()
DATEDIFF()
DATE_FORMAT()
```

These functions help extract and format useful information from dates.

---

### ✏️ 4. String Functions

The following functions are demonstrated:

```sql
CONCAT()
REPLACE()
UPPER()
LOWER()
TRIM()
```

They are used for formatting and cleaning text data.

---

### 📈 5. Window Functions

The project demonstrates:

```sql
SUM() OVER()
RANK() OVER()
```

These are used for:

* Running totals
* Ranking orders

---

### 🏷️ 6. CASE Statements

`CASE` is used to categorize data.

Examples:

* Order discount categories
* Employee salary categories

---

# 📋 17 SQL Queries

|  # | Query Concept                  |
| -: | ------------------------------ |
| 01 | INNER JOIN                     |
| 02 | LEFT JOIN                      |
| 03 | RIGHT JOIN                     |
| 04 | FULL OUTER JOIN using UNION    |
| 05 | Above-Average Order Customers  |
| 06 | Above-Average Salary Employees |
| 07 | Extract Year & Month           |
| 08 | Date Difference                |
| 09 | Date Formatting                |
| 10 | Concatenate Full Name          |
| 11 | Replace Text                   |
| 12 | Uppercase & Lowercase          |
| 13 | Trim Email                     |
| 14 | Running Total                  |
| 15 | Ranking                        |
| 16 | Order Discount                 |
| 17 | Salary Category                |

---

# 💡 Important Concept

### Why is `UNION` used in Query 4?

MySQL/MariaDB does not directly support `FULL OUTER JOIN`.

Therefore:

```text
LEFT JOIN
     +
RIGHT JOIN
     +
UNION
     ↓
FULL OUTER JOIN-like Result
```

`UNION` combines the results of the two JOIN operations into one result set.

---

# 🚀 How to Run This Project

### Step 1️⃣ Start XAMPP

Open **XAMPP Control Panel** and start:

```text
Apache
MySQL
```

### Step 2️⃣ Open phpMyAdmin

Open phpMyAdmin from your browser.

### Step 3️⃣ Create Database

Run:

```sql
CREATE DATABASE data_transformer;
USE data_transformer;
```

### Step 4️⃣ Create Tables

Create the following tables:

```text
Customers
Orders
Employees
```

### Step 5️⃣ Insert Data

Insert the project data into each table.

### Step 6️⃣ Execute Queries

Run the **17 SQL queries** one by one in phpMyAdmin.

---

# 📊 Expected Learning Outcomes

After completing this project, you will understand:

✅ SQL JOIN operations
✅ Subqueries
✅ Date functions
✅ String functions
✅ Window functions
✅ Ranking
✅ Running totals
✅ Conditional statements
✅ Data transformation
✅ Basic database analysis

---

# 🎓 Project Type

**Academic / Practical SQL Project**

### Suitable For:

* 📚 College Practical
* 🧪 SQL Lab Work
* 🎓 Database Management System
* 💻 MySQL Practice
* 📝 Viva Preparation
* 📂 Mini Project

---

# 👩‍💻 Author

**MINAXI CHOUDHARI**

> 💻 Learning SQL • Database Management • Data Transformation

---

## ⭐ Project Highlights

```text
17 SQL Queries
      ↓
3 Database Tables
      ↓
JOINs + Subqueries
      ↓
Date + String Functions
      ↓
Window Functions
      ↓
CASE Statements
      ↓
Data Analysis
```

---

###  Thank You



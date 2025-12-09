# 🗄️ Employee Database SQL Script

This repository contains an SQL script that creates and populates an **Employee Database**, along with multiple example queries demonstrating filtering, pattern matching, and NULL handling in SQL.

---

## 📌 Overview

The SQL file performs the following operations:

### ✔️ 1. Create Database & Table
- Creates a database named **employees**
- Creates a table **Employees** with:
  - `employee_id` (Primary Key)
  - `name`
  - `age`
  - `department`

### ✔️ 2. Insert Sample Data
The script inserts **100 sample employee records** covering:
- Multiple departments (Sales, Marketing, HR, Finance, Operations)
- NULL values in fields like age and department
- Realistic dataset for SQL practice

### ✔️ 3. SQL Queries Included

#### 🔹 Basic Queries
- `SELECT * FROM Employees;`
- Conditional filtering using `WHERE`, `AND`, `OR`

#### 🔹 Conditional Filtering
- Employees older than 30  
- Employees from Sales & Marketing  
- Employees within age ranges  
- Using **BETWEEN** to simplify range queries

#### 🔹 Pattern Matching
Use of `LIKE` for name-based search:
```sql
SELECT * FROM Employees WHERE name LIKE 'J%';

```
####🔹 NULL Handling
```
SELECT * FROM Employees WHERE department IS NULL;
SELECT * FROM Employees WHERE age IS NOT NULL;
```

####🔹 IN / NOT IN Usage
```
SELECT * FROM Employees 
WHERE department IN ('Sales', 'Marketing');

SELECT * FROM Employees 
WHERE department NOT IN ('Sales', 'Marketing');

```
📄 License

This project is open-source and free to use.

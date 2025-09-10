# 🛒 Retail Data Analysis – Advanced SQL Concepts  

## 📌 Overview  
This project explores a **Retail dataset** using **advanced SQL queries** to perform data preparation, cleaning, and deep analysis.  
The goal is to uncover insights on **customers, transactions, product categories, and revenue patterns** while applying **SQL best practices and advanced techniques** such as:  

- Joins  
- CTEs (Common Table Expressions)  
- Aggregations & Grouping  
- Window Functions  
- Date transformations  

This demonstrates the power of **SQL alone** in handling complex analytical tasks in real-world business scenarios.  

---

## 🎯 Objectives  
- Clean and prepare retail data (dates, null handling, transformations).  
- Explore **customer demographics and behavior**.  
- Analyze **transaction trends** (sales vs returns, time range, store types).  
- Identify **high-value categories and subcategories**.  
- Understand **revenue contribution by customers and channels**.  
- Apply **advanced SQL logic** to solve business-driven queries.  

---

## ⚙️ Tools & Technologies  
- **SQL Server** (T-SQL) / Any RDBMS with SQL support  
- Concepts used:  
  - `JOIN`, `GROUP BY`, `HAVING`  
  - `CTEs` for reusable logic  
  - `DATEDIFF`, `DATEADD` for time-based analysis  
  - Subqueries & Nested queries  
  - Aggregations (`SUM`, `COUNT`, `AVG`, `MAX`, `MIN`)  

---

---

## 📊 Key Insights  

### 1. Data Preparation  
- Converted incorrect **transaction dates** into valid SQL date format.  
- Found **time range of data** in **days, months, and years**.  

**SQL Snippet:**  
```sql
select 
DATEDIFF(YEAR, min(CONVERT(date, tran_date,105)), max(CONVERT(date, tran_date,105))) as TOTAL_YEAR,
DATEDIFF(MONTH, min(CONVERT(date, tran_date,105)) ,max(CONVERT(date, tran_date,105))) as TOTAL_MONTHS,
DATEDIFF(DAY,min(CONVERT(date, tran_date,105)),max(CONVERT(date, tran_date,105))) as TOTAL_DAYS
from Transactions;


## 📂 Project Structure  


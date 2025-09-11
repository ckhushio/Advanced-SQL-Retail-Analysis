# 🛒 Retail Data Analysis – Using Advanced SQL Concepts  

## 📑 Project Overview  
This project explores a retail database using advanced SQL techniques. Three tables—**Customer**, **Transactions**, and **prod_cat_info**—were analyzed to uncover business insights, including sales performance, customer behavior, and product category trends.  

---

## 🗂️ Dataset Structure  
- **Customer**: Customer demographics (ID, Gender, DOB, City).  
- **Transactions**: Purchase and return records (transaction ID, cust_id, qty, total_amt, tran_date, store_type).  
- **prod_cat_info**: Product category and sub-category mapping.  

---

## 🧹 Data Preparation  
- Converted dates to valid formats (`CONVERT(date, tran_date, 105)`).  
- Checked row counts for all three tables.  
- Cleaned negative quantities to identify **returns**.  
- Created CTEs and subqueries for advanced calculations (e.g., age-based filtering, category averages).  

---

## 📊 Key Analyses & Queries  
1. **Data Overview**  
   - Counted total rows per table.  
   - Calculated the **time range** of transactions (in days, months, years).  
   - Found the product category for the sub-category “DIY.”  

2. **Customer & Sales Insights**  
   - Counted **male vs. female** customers.  
   - Identified the **city** with the maximum customers.  
   - Found customers with **>10 transactions** (excluding returns).  
   - Computed net revenue for **25–35-year-olds** in the last 30 days.  

3. **Product & Category Insights**  
   - Counted **Books** subcategories.  
   - Found the **maximum quantity** of products ever ordered.  
   - Calculated revenue for **Electronics** and **Books** categories.  
   - Determined **combined revenue** from Electronics & Clothing in flagship stores.  
   - Identified **categories with average revenue above overall average**.  

4. **Returns & Fulfilment**  
   - Counted total **returns**.  
   - Found the product category with the **highest returns** in the last 3 months.  
   - Analyzed **store-types** for maximum quantity sold and value of sales.  
   - Calculated **percentage of sales vs returns** for top 5 subcategories.  

5. **Top Performers**  
   - Ranked **top 5 categories by quantity sold**.  
   - Calculated **average and total revenue** by subcategory within these top categories.  

---

## 🔍 Findings  
- **Electronics and Books** are top revenue generators.  
- **Flagship stores** drive significant sales for high-value categories.  
- **DIY** belongs to a specific product category, highlighting niche demand.  
- Most transactions are **B2C**, and **returns** are relatively low but concentrated in specific categories.  
- Customers aged **25–35** contribute notable revenue, especially in the most recent 30-day period.  
- A few **store types** dominate in both quantity and value of sales.  

---

## 🧭 Practical Recommendations  
1. **Boost Electronics & Books Campaigns:** Increase marketing spend and stock levels for these high-performing categories.  
2. **Improve Flagship Store Strategy:** Optimize flagship store operations and promotions for Electronics and Clothing.  
3. **Target Young Adults:** Create loyalty offers for the **25–35 age group**—a high-value segment.  
4. **Address High-Return Categories:** Review product descriptions and logistics for categories with high return values.  
5. **Expand High-Performing Store Types:** Replicate successful store models in underperforming areas.  
6. **Optimize Subcategories:** Focus on top subcategories with high sales-to-return ratios.  

---

## 🧰 SQL Concepts Used  
- **Window Functions** (e.g., `DATEDIFF`, `DATEADD`).  
- **Aggregate Functions** (`SUM`, `COUNT`, `AVG`, `MAX`).  
- **Joins** (INNER, LEFT, RIGHT).  
- **Common Table Expressions (CTEs)** for filtering and advanced calculations.  
- **GROUP BY & HAVING** for grouped metrics.  
- **Subqueries** for nested calculations.  

---

## 📌 How to Use  
1. Import the SQL script into your database (e.g., SQL Server).  
2. Run each query step by step to replicate the analysis.  
3. Optionally, export results into Power BI or Excel for visualization.  

---

✨ *This analysis demonstrates the power of advanced SQL techniques for uncovering actionable business insights in retail data.*  

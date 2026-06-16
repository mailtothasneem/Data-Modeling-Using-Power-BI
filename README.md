## Data-Modeling-Using-Power-BI
 
  This Power BI analysis solves the business problem of comparing actual sales performance against defined monthly and category‑wise targets to identify gaps and guide better decision‑making.
    
 #🎯 Project Overview
 Business Problem:

  The organization struggled to track and evaluate actual sales performance against predefined monthly and category‑wise targets, making it difficult to identify shortfalls, measure profitability, and support informed decision‑making.
     
 # Objective:

  The objective of this project is to transform raw sales data into a clean, structured model in Power BI that enables accurate performance analysis. Specifically, the project aims to:
- Clean and prepare datasets (Orders, Order Details, Sales Target) using Power Query.
- Apply transformations such as text formatting, column creation, conditional logic, grouping, and merging.
  
# Target Audience:

 - Executive Leadership → to monitor overall sales performance against strategic targets.
 - Sales Operations Teams → to track category‑wise and monthly performance, identify shortfalls, and adjust sales strategies.

 # 🗃️ Data Sources & Architecture

   Source Systems :
   
      Power Query → Used for data transformation, cleaning, and preparation before loading into Power BI.
      Power BI Desktop → The main environment for modeling relationships and building dashboards.
    
Data Volume:

  -Orders Dataset (List of Orders.csv) → ~2,000 rows of customer orders spanning April 2018 – March 2019.
  -Order Details Dataset (Order Details.csv) → ~500 rows of product‑level details (Amount, Profit, Quantity, Category,Sub‑Category).
 -Sales Target Dataset (Sales target.csv) → 36 rows of monthly category‑wise targets (Furniture, Clothing, Electronics).
 -Timeframe Covered → One full business year of sales transactions and targets.
 
Storage Mode: This project uses Import Mode in Power BI.

# ⚙️ Data Transformation (ETL)

   -Tool Used : Power Query Editor.
Key Cleanups:
   - Standard transformations applied to raw data in Power Query include:
   - Merging Queries → Combined Orders and Order Details using Order ID as the key.
   - Column Creation → Added calculated columns for Total Sales, Profit Margin, and *Target Achievement %.

 # 🧠 Data Model 

  Model Type - Star Schema
  The design centers on a single fact table (Sales Fact) linked to multiple dimension tables for simplicity and 
  performance.
 
  Fact Tables:
  
  -Order Details →Transactional sales data (Amount, Profit, Quantity, Category, Sub‑Category).
  -Sales Target → Monthly targets by category.

  Dimension Tables
  
   -Orders → Customer, State, City, and Order Date.
  -Product Dimension → Product details (Category, Sub‑Category, Brand).
  -Date Table → Dedicated calendar table for time intelligence (Year, Month, Quarter).

 # 🖥️ Dashboard Features

  -The Power BI dashboard provides the following capabilities:
  - Sales vs Target Analysis → Compare actual sales against monthly and category‑wise targets.
  -Profitability Insights → Track total profit, profit margin %, and identify loss‑making products.

# 🚀 How To Use

-Install Power BI Desktop
-Ensure you have the latest version of Power BI Desktop installed for full functionality.
-Download from Microsoft Power BI official site
-Verify installation is complete
-Open Power BI Desktop to confirm version.

             Thank You

# SQL Data Analytics Project  

**Retail Business Analytics using SQL Server — Customer Segmentation, Product Performance & Trend Analysis**

---

## Project Overview

This project demonstrates advanced SQL-based business analytics performed on a structured retail dataset.

The analysis is conducted on the **Gold Layer** of a previously developed SQL Data Warehouse (Medallion Architecture implementation), enabling high-performance analytical querying using fact and dimension tables.

This repository focuses on translating modeled warehouse data into actionable business insights through structured SQL analysis.

---

## Built on Top of Data Warehouse

This project builds upon the SQL Data Warehouse developed in the companion repository:

https://github.com/Pratha-Joshi/sql-data-warehouse-project

The analytics queries leverage the **Star Schema (Fact and Dimension tables)** from the Gold layer.

Together, both repositories simulate a real-world workflow:

**Raw Data → Data Engineering → Data Modeling → Business Analytics**

---

## Business Objectives

Retail businesses need to understand:

- Who are the most valuable customers?
- Which products drive the highest revenue?
- How does sales performance change over time?
- Which segments contribute most to profitability?

This project answers these questions using structured SQL queries designed for performance and clarity.

---

# Customer Report

## Purpose

To consolidate key customer metrics and behavioral insights that support segmentation, retention strategies, and revenue optimization.

## Key Analysis Performed

### Customer Data Consolidation
- Extracted core attributes such as name, age, and transaction details  
- Structured joins across fact and dimension tables  

### Customer Segmentation
Customers were grouped into 3 segments based on spending behavior:

- **VIP** → At least 12 months of history AND spending > $5000  
- **Regular** → At least 12 months of history AND spending ≤ $5000  
- **New** → Lifespan < 12 months  

Customers were also categorized into age groups to analyze demographic trends.

### Aggregated Customer Metrics
- Total orders  
- Total sales  
- Total quantity purchased  
- Total unique products purchased  
- Customer lifespan (in months)

### Customer KPIs Calculated
- Recency (months since last order)  
- Average Order Value (AOV)  
- Average Monthly Spend  

These metrics help identify high-value customers and retention opportunities.

---

# Product Report

## Purpose

To evaluate product performance, revenue contribution, and lifecycle trends.

## Key Analysis Performed

### Product Data Consolidation
- Extracted product name, category, subcategory, and cost  

### Revenue-Based Segmentation
Products were categorized into:
- High Performers  
- Mid-Range  
- Low Performers  

### Aggregated Product Metrics
- Total orders  
- Total sales  
- Total quantity sold  
- Total unique customers  
- Product lifespan (in months)

### Product KPIs Calculated
- Recency (months since last sale)  
- Average Order Revenue (AOR)  
- Average Monthly Revenue  

These insights help monitor product lifecycle and profitability.

---

# Exploratory & Trend Analysis

Additional analytical queries include:

- Monthly sales trends and running totals  
- Year-over-year product performance comparison  
- Comparison of yearly sales vs product average sales  
- Category contribution to overall revenue  
- Product cost range segmentation  
- Customer distribution across spending segments  

These analyses simulate real-world BI use cases such as revenue forecasting, product lifecycle management, and customer value analysis.

---

## Business Impact

The analytical reports in this project help:

- Identify high-value customers for targeted marketing  
- Monitor revenue concentration and customer retention  
- Evaluate product performance across categories  
- Support data-driven strategic decisions  

---

## Dataset

The retail dataset used in this project was obtained from a publicly available SQL analytics tutorial by Data With Baraa.

The warehouse modeling, analytical queries, segmentation logic, and documentation were implemented independently as part of hands-on practice in data engineering and business analytics.




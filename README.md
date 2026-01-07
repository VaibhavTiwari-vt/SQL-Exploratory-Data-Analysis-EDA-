# Sales Analytics Using SQL  
**Exploratory Data Analysis & Advanced Business Analytics**

---

## 📌 Project Overview
This repository contains an end-to-end **SQL-based data analytics project** designed to answer real-world business questions using sales data. The project covers both **Exploratory Data Analysis (EDA)** and **Advanced Analytics**, following best practices used in data analytics and business intelligence roles.

The analysis is performed on a **star-schema data warehouse** using fact and dimension tables and demonstrates how SQL can be used not only for querying data, but for **business insights, performance analysis, segmentation, and reporting**.

---

## 🏗️ Data Model

### Fact Table
- **`gold.fact_sales`**
  - Transaction-level sales data
  - Measures: `sales_amount`, `quantity`, `price`, `order_date`, `order_number`

### Dimension Tables
- **`gold.dim_customers`**
  - Customer demographics (name, age, gender, country, birthdate)
- **`gold.dim_products`**
  - Product details (product name, category, subcategory, cost)

---

## 🔍 Exploratory Data Analysis (EDA)

The EDA phase focuses on understanding the structure, scale, and distribution of the data.

### 1. Database & Schema Exploration
- Explored all tables and columns using `INFORMATION_SCHEMA`
- Validated fact–dimension relationships

### 2. Dimension Exploration
- Customer distribution by country and gender
- Product hierarchy exploration (category, subcategory, product)
- Youngest and oldest customers based on birthdate

### 3. Date Exploration
- Identified first and last order dates
- Calculated total years of sales history available

### 4. Measures & Key Metrics
Computed core business KPIs:
- Total sales revenue
- Total items sold
- Average selling price
- Total orders and distinct orders
- Total customers
- Customers who placed at least one order

A consolidated KPI report was generated using `UNION ALL` for easy business reporting.

### 5. Magnitude Analysis
- Customers by country and gender
- Products by category
- Average product cost per category
- Revenue by category
- Revenue by customer
- Quantity sold by country

### 6. Ranking Analysis
- Top 5 products by revenue
- Bottom 5 worst-performing products

---

## 📈 Advanced Data Analytics

The advanced analytics section applies analytical SQL techniques commonly used in BI and decision support systems.

### 1. Change Over Time (Trend Analysis)
- Monthly and yearly sales trends
- Customer growth over time
- Quantity sold trends using `DATETRUNC`

### 2. Cumulative & Moving Average Analysis
- Monthly sales with running totals
- Yearly cumulative sales
- Moving average of selling price

### 3. Performance Analysis
- Year-over-year (YoY) product sales comparison
- Product performance vs historical average
- Performance classification:
  - Above Average / Below Average
  - Increase / Decrease / No Change

### 4. Part-to-Whole Analysis
- Category contribution to total sales
- Percentage share of overall revenue

### 5. Segmentation Analysis

#### Product Segmentation
Products segmented by cost range:
- Below 100  
- 100–500  
- 500–1000  
- Above 1000  

#### Customer Segmentation
Customers classified as:
- **VIP**: ≥12 months lifespan & spending > $5000
- **Regular**: ≥12 months lifespan & spending ≤ $5000
- **New**: <12 months lifespan

---

## 📊 Reporting Layer (SQL Views)

To support dashboards and business reporting, two analytical views were created.

### 1. `gold.report_customers`
Provides:
- Customer demographics and age groups
- Customer segmentation (VIP / Regular / New)
- Recency and lifespan
- Total orders, sales, quantity, and products purchased
- Average order value
- Average monthly spend

### 2. `gold.report_products`
Provides:
- Product hierarchy and cost
- Sales lifespan and recency
- Product performance segmentation
- Total orders, customers, sales, and quantity
- Average selling price
- Average order revenue and monthly revenue

---

## 🎯 Business Questions Answered
- Which products and categories generate the most revenue?
- How does sales performance change over time?
- Who are the most valuable customers?
- Which products are underperforming?
- How is revenue distributed across categories?
- How should customers and products be segmented for strategy?

---

## 🛠️ Tools & Skills Demonstrated
- Advanced SQL (CTEs, window functions, ranking, aggregation)
- Time-series analysis
- Customer and product segmentation
- KPI design and reporting
- Data warehousing concepts
- Business-focused analytical thinking

---

## 👤 About Me
**Vaibhav Tiwari**  
Final-year student at **Punjab Engineering College**  

I am passionate about data analytics and business intelligence, with a strong interest in using SQL and data-driven approaches to solve real-world business problems. This project reflects my hands-on experience with analytical SQL, data warehousing concepts, and translating data into actionable insights.





## 📁 Repository Structure (Suggested)

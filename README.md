# Sales Performance Dashboard 📊

## Project Overview

The **Sales Performance Dashboard** is a Business Analytics project developed using **Power BI, Excel, and SQL** to analyze sales performance and generate meaningful business insights.

The dashboard helps businesses understand revenue trends, product performance, regional sales, and customer behavior to support data-driven decision-making.

---

## Business Problem

A company wants to analyze its sales data to answer important business questions:

- What are the total sales and profit generated?
- Which products and categories perform best?
- Which regions contribute the highest revenue?
- Who are the top customers?
- How do sales trends change over time?

This dashboard provides visual insights to help management make better business decisions.

---

## Objectives

- Analyze overall sales performance.
- Identify profitable products and categories.
- Understand regional sales performance.
- Analyze customer purchasing patterns.
- Create interactive reports for decision-making.

---

# Tools & Technologies

| Tool | Purpose |
|---|---|
| Power BI | Dashboard development and data visualization |
| Excel | Data cleaning and preparation |
| Power Query | Data transformation |
| DAX | Creating calculated measures |
| SQL Server / T-SQL | Data analysis and querying |

---

# Dataset

**Dataset Name:** Superstore Sales Dataset

**Source:** Kaggle

The dataset contains sales transaction details including:

- Order ID
- Order Date
- Customer Information
- Product Details
- Category
- Region
- Sales
- Quantity
- Profit

---

# Data Preparation

The raw dataset was cleaned and prepared before analysis.

Data cleaning steps:

✅ Removed empty rows  
✅ Checked and corrected date formats  
✅ Removed duplicate records  
✅ Handled missing values  
✅ Converted data into structured tables  
✅ Prepared data for Power BI analysis  

---

# Dashboard Features

## 1. Sales Overview Dashboard

Key KPIs:

- Total Sales
- Total Profit
- Total Orders
- Profit Margin

Visualizations:

- Monthly Sales Trend
- Sales by Category
- Sales by Segment
- Profit Analysis


## 2. Customer Analysis Dashboard

Includes:

- Top Customers by Sales
- Customer Segment Analysis
- Customer Purchasing Trends


## 3. Regional Analysis Dashboard

Includes:

- Sales by Region
- Regional Profit Comparison
- Geographic Sales Distribution

---

# DAX Measures Created

### Total Sales

```DAX
Total Sales =
SUM(Sales_Data[Sales])
```

### Total Profit

```DAX
Total Profit =
SUM(Sales_Data[Profit])
```

### Total Orders

```DAX
Total Orders =
COUNT(Sales_Data[Order ID])
```

### Profit Margin

```DAX
Profit Margin =
DIVIDE(
SUM(Sales_Data[Profit]),
SUM(Sales_Data[Sales])
)
```

---

# SQL Analysis

Sample SQL queries used for business analysis:

## Total Sales

```sql
SELECT 
SUM(Sales) AS Total_Sales
FROM Sales_Data;
```

## Sales by Category

```sql
SELECT
Category,
SUM(Sales) AS Revenue
FROM Sales_Data
GROUP BY Category;
```

## Top Customers

```sql
SELECT TOP 10
Customer_Name,
SUM(Sales) AS Total_Revenue
FROM Sales_Data
GROUP BY Customer_Name
ORDER BY Total_Revenue DESC;
```

---

# Key Business Insights

Example insights generated from the dashboard:

- The Technology category generated the highest revenue.
- Certain regions contributed more sales compared to others.
- High sales products did not always generate the highest profit.
- Customer segments showed different purchasing patterns.
- Sales trends changed throughout the year, showing seasonal patterns.

---

# Project Structure

```
Sales-Performance-Dashboard/
│
├── Dataset/
│   └── Sales_Data_Cleaned.xlsx
│
├── PowerBI/
│   └── Sales_Performance_Dashboard.pbix
│
├── SQL/
│   └── Sales_Analysis.sql
│
├── Images/
│   └── dashboard.png
│
└── README.md
```

---

# Skills Demonstrated

- Business Intelligence
- Data Cleaning
- Data Visualization
- Dashboard Development
- SQL Data Analysis
- Power BI Reporting
- Business Insights Generation

---

# Author

**Kaveesha Maharambage**



# Superstore Sales Executive Dashboard | Power BI

## 📌 Project Overview

The **Superstore Sales Executive Dashboard** is an interactive business intelligence project developed using Microsoft Power BI to analyze sales performance, profitability, product categories, regional performance, and business trends.

The project transforms raw sales transaction data into meaningful insights through KPI scorecards, interactive visualizations, and dynamic filters. It is designed to help business stakeholders and executives monitor performance, identify growth opportunities, and make data-driven decisions.

---

## 🎯 Problem Statement

Businesses need an effective way to monitor sales performance, evaluate profitability, identify high-performing products and regions, and understand year-over-year business trends.

The objective of this project is to transform raw Superstore sales records into an interactive executive dashboard that provides a clear overview of business performance through key performance indicators (KPIs), trend analysis, and product and regional performance visualizations.

---

## 🎯 Project Objectives

- Analyze overall sales and profit performance.
- Track key business KPIs through executive scorecards.
- Evaluate monthly sales trends and year-over-year growth.
- Analyze sales performance across categories and sub-categories.
- Identify regional performance patterns.
- Monitor profitability and profit margins.
- Enable interactive exploration through date and region slicers.
- Present business insights in a professional and user-friendly dashboard.

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| Microsoft Power BI Desktop | Dashboard development and visualization |
| Power Query | Data cleaning, transformation, and preparation |
| DAX (Data Analysis Expressions) | KPI calculations and business metrics |
| Data Modeling | Organizing data for analytical reporting |
| CSV Dataset | Source sales transaction data |
| GitHub | Project documentation and portfolio presentation |

---

## 📊 Dataset Description

The project uses a Superstore sales dataset containing transaction-level sales information.

| Dataset Information | Details |
|---|---|
| Dataset Name | Superstore Sales |
| File Format | CSV |
| Total Records | 10,800 |
| Total Columns | 21 |
| Data Type | Sales transaction data |

### Key Dataset Fields

- **Order Information:** Row ID, Order ID, Order Date, Ship Date, Ship Mode
- **Customer Information:** Customer ID, Customer Name, Segment
- **Geographic Information:** Country, City, State, Postal Code, Region
- **Product Information:** Product ID, Category, Sub-Category, Product Name
- **Sales Metrics:** Sales, Quantity, Discount, Profit

---

## 📈 Dashboard Features

### 1. Executive KPI Scorecards

Provides a quick overview of business performance using key metrics:

- **Total Sales** – Overall revenue generated from sales.
- **Total Profit** – Total profit earned across transactions.
- **Total Orders** – Number of orders placed.
- **Profit Margin %** – Measures profitability as a percentage of total sales.
- **YoY Sales Growth %** – Measures the percentage increase or decrease in sales compared with the previous year.

These KPIs help executives quickly assess the overall performance of the business.

### 2. Monthly Sales Trend Analysis

A line chart visualizes sales performance over time, helping identify:

- Monthly sales fluctuations
- Sales trends and seasonality
- High- and low-performing months
- Year-over-year sales performance

### 3. Category & Sub-Category Treemap

The treemap provides a visual breakdown of product performance across categories and sub-categories.

- **Category:** Product category
- **Details:** Sub-category
- **Values:** Previous Year Sales
- **Tooltips:** Total Sales and Total Profit

This visualization helps compare product groups and understand their contribution to business performance.

### 4. Interactive Date Slicer

Allows users to filter dashboard data by date and analyze performance across different time periods.

### 5. Regional Performance Analysis

An interactive region slicer enables users to explore sales and profitability for different geographic regions and compare regional business performance.

---

## 🧮 Key DAX Measures

The following measures are used or planned as core analytical calculations for the dashboard.

### Total Sales

```dax
Total Sales = SUM(Orders[Sales])
```

### Total Profit

```dax
Total Profit = SUM(Orders[Profit])
```

### Total Orders

```dax
Total Orders = DISTINCTCOUNT(Orders[Order ID])
```

### Profit Margin %

```dax
Profit Margin % =
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)
```

### Previous Year Sales

```dax
Previous Year Sales =
CALCULATE(
    [Total Sales],
    SAMEPERIODLASTYEAR('Date'[Date])
)
```

### YoY Sales Growth %

```dax
YoY Sales Growth % =
DIVIDE(
    [Total Sales] - [Previous Year Sales],
    [Previous Year Sales],
    0
)
```

---

## 🗂️ Data Modeling Approach

The recommended analytical model follows a **Star Schema** structure to improve organization, maintainability, and analytical performance.

### Fact Table

**Fact Orders**

Contains transactional sales information such as:

- Order ID
- Order Date
- Customer ID
- Product ID
- Sales
- Quantity
- Discount
- Profit

### Dimension Tables

**Dim Customer**
- Customer ID
- Customer Name
- Segment

**Dim Product**
- Product ID
- Product Name
- Category
- Sub-Category

**Dim Date**
- Date
- Year
- Quarter
- Month
- Month Number

The dimension tables provide descriptive information for filtering and grouping, while the fact table contains transaction-level metrics.

---

## 💡 Business Value

The dashboard supports business decision-making by helping stakeholders:

- Monitor revenue and profit performance.
- Understand sales trends over time.
- Compare current performance with previous-year performance.
- Identify profitable product categories and sub-categories.
- Evaluate regional sales performance.
- Understand profit margins and profitability.
- Explore performance interactively using slicers.

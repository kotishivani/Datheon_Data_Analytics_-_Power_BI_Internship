# Exploratory Data Analysis (EDA) on Superstore Retail Sales

## Project Overview

This project focuses on analyzing Superstore sales data using Python to identify business trends, customer purchasing patterns, regional performance, product category performance, and the relationship between discounts and profitability.

The analysis is performed using Python libraries such as Pandas, NumPy, Matplotlib, Seaborn, and Plotly. Data cleaning, exploratory data analysis (EDA), statistical analysis, and data visualization techniques are used to transform raw sales data into meaningful business insights.

The main objective is to understand sales performance, identify profitable business areas, and provide data-driven recommendations to support better business decisions.

## Project Objectives

- Analyze customer purchase volume based on total orders, sales, and quantity purchased.
- Identify monthly sales trends and seasonal patterns.
- Evaluate sales and profitability across different product categories.
- Compare regional sales and profit performance.
- Analyze sales contributions from different customer segments.
- Understand the relationship between discounts and profitability.
- Identify key business insights and recommendations.

## Tools and Technologies Used

| Tool / Library | Purpose |
|---|---|
| Python | Data analysis and programming |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical data visualization |
| Plotly | Interactive visualizations |
| Jupyter Notebook | Development and analysis environment |

## Dataset Description

The project uses the Superstore Sales dataset containing information about customer orders, products, sales, discounts, and profits.

The dataset includes the following important columns:

- Order ID – Unique identifier for customer orders.
- Order Date – Date when the order was placed.
- Customer ID – Unique identifier for customers.
- Customer Name – Name of the customer.
- Segment – Customer segment.
- Region – Geographical sales region.
- Category – Product category.
- Sub-Category – Product sub-category.
- Sales – Sales amount.
- Quantity – Number of products purchased.
- Discount – Discount applied to the order.
- Profit – Profit or loss generated from the order.

## Project Workflow

### 1. Data Loading and Initial Inspection

- Imported the required Python libraries.
- Loaded the Superstore Sales dataset using Pandas.
- Examined the dataset using `head()`, `shape`, `info()`, and `describe()`.
- Identified the number of records, columns, data types, and statistical information.

### 2. Data Cleaning and Preprocessing

- Identified and removed duplicate records.
- Checked missing values in the dataset.
- Filled missing numerical values using the median.
- Filled missing categorical values using the mode.
- Converted the Order Date column into datetime format.
- Extracted Year, Month, and Year-Month columns for time-based analysis.

### 3. Exploratory Data Analysis (EDA)

Performed the following analyses:

**Customer Purchase Analysis**
- Calculated the total number of unique orders for each customer.
- Analyzed total sales and quantities purchased.
- Identified the top 10 customers based on sales.

**Category-wise Sales and Profit Analysis**
- Compared total sales, profit, and quantity across product categories.
- Identified the highest revenue-generating category.
- Evaluated category-wise profitability.

**Region-wise Sales and Profit Analysis**
- Analyzed sales and profit across the Central, East, South, and West regions.
- Identified the highest-performing region.

**Customer Segment Analysis**
- Compared sales, profit, and quantity across Consumer, Corporate, and Home Office segments.
- Evaluated the contribution of each customer segment.

**Monthly Sales Trend Analysis**
- Aggregated sales by Year-Month.
- Identified monthly sales patterns.
- Visualized sales trends using an interactive line chart.

**Discount vs Profit Analysis**
- Examined the relationship between discounts and profits.
- Created a scatter plot to understand discount sensitivity.
- Calculated the correlation between discount and profit.

## Key Business Insights

The analysis produced the following important business findings:

1. **Category Performance:** Technology generated the highest sales of approximately $836,154, followed by Furniture and Office Supplies. Furniture recorded comparatively lower profitability.

2. **Regional Performance:** The West region recorded the highest sales of approximately $741,914 and the highest profit of approximately $111,036. The East region generated approximately $678,781 in sales.

3. **Customer Segment:** The Consumer segment contributed the highest sales of approximately $1.18 million, followed by Corporate with approximately $706,146. Home Office generated the lowest sales but achieved the highest profit margin.

4. **Monthly Sales Trends:** November 2018 recorded the highest monthly sales of approximately $118,447.83, while February 2015 recorded the lowest monthly sales of approximately $4,519.89.

5. **Discount vs Profit:** The correlation between Discount and Profit was approximately -0.22, indicating a negative relationship between discount levels and profitability.

## Data Visualizations

The project includes the following visualizations to communicate business performance:

- Category-wise Sales Analysis – Compares sales across product categories.
- Region-wise Sales Analysis – Displays regional sales performance.
- Customer Segment-wise Sales Analysis – Compares sales contributions by customer segment.
- Monthly Sales Trend – Displays monthly sales variations using an interactive line chart.
- Discount vs Profit Analysis – Illustrates the relationship between discounts and profits using a scatter plot.

## Conclusion

The Superstore Sales Analysis highlights the importance of understanding customer purchasing behavior, product performance, regional contributions, and discount strategies.

Technology, the West region, and the Consumer segment were the major contributors to sales performance.

Based on the findings, the business should focus on improving Furniture profitability, controlling excessive discounts, and increasing sales during low-performing months.

This project demonstrates practical skills in Python programming, data cleaning, exploratory data analysis, data visualization, and business insight generation.

## How to Run the Project

1. Clone or download this repository.
2. Install Python and Jupyter Notebook.
3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn plotly kaleido
```

4. Place the `superstore_sales.csv` dataset in the project directory or update its file path in the notebook.
5. Open the Jupyter Notebook:

```bash
jupyter notebook
```

6. Open `Superstore_Sales_Analysis.ipynb`.
7. Run the notebook cells sequentially to reproduce the analysis and visualizations.

## Skills Demonstrated

- Python Programming
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Data Aggregation and Grouping
- Statistical Analysis
- Data Visualization
- Business Insights and Interpretation
- Analytical Thinking and Problem Solving

---

**Project Category:** Data Analytics

**Programming Language:** Python

**Development Environment:** Jupyter Notebook

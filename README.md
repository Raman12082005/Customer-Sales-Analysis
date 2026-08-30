# Customer Sales Analysis

## 📌 Overview

This project performs a business-focused exploratory data analysis (EDA) of a customer sales dataset.

The objective is to understand the company's sales and profitability performance across different categories, regions, customer segments, products, time periods, and discount levels.

The project follows a practical data analyst workflow:

**Data Understanding → Data Cleaning → KPI Analysis → Exploratory Analysis → Visualization → Relationship Analysis → Business Insights → Recommendations**

The analysis focuses not only on identifying what happened in the data, but also on understanding what the findings could mean from a business perspective.

---

## 🎯 Business Objective

The primary objective of this project is to analyze historical customer sales data and identify patterns that can help a business understand its revenue and profitability performance.

### Key Business Questions

- Which product categories generate the most revenue?
- Which regions generate the most sales and profit?
- Which customer segments contribute the most revenue?
- Which products are the strongest and weakest performers?
- How have sales changed over time?
- Are there seasonal sales patterns?
- Is there an association between discount levels and profitability?
- Which areas require further business investigation?
- What recommendations can be made based on the analysis?

---

## 📊 Dataset

The dataset contains transactional sales information covering products, customers, locations, sales, profit, discounts, shipping, and order information.

### Main Data Fields

- Category
- Sub-Category
- Product ID
- Product Name
- Customer ID
- Customer Name
- Sales
- Profit
- Quantity
- Discount
- Region
- Market
- Country
- State
- City
- Segment
- Order Date
- Shipping Date
- Shipping Mode
- Shipping Cost
- Order Priority

### Dataset Scale

The dataset contains more than **51,000 sales records**, covering more than **25,000 orders** and approximately **4,800 customers**.

---

## 🛠️ Technologies Used

- **Python**
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical analysis
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Jupyter Notebook** — Interactive analysis environment

---

## 🔍 Analysis Performed

### 1. Data Understanding

- Dataset shape and dimensions
- Data types
- Statistical summary
- Unique-value analysis
- Missing-value analysis
- Duplicate-record analysis

### 2. Data Cleaning

- Date conversion
- Redundant-column investigation
- Removal of non-informative columns where appropriate
- Creation of time-based features
- Calculation of shipping duration

### 3. Business KPI Analysis

Calculated key business metrics including:

- Total Sales
- Total Profit
- Profit Margin
- Total Quantity Sold
- Number of Unique Orders
- Number of Unique Customers

### 4. Sales Analysis

Analyzed:

- Sales by Category
- Sales by Region
- Sales by Customer Segment
- Sales by Year
- Monthly Sales Patterns
- Top 10 Products by Sales

### 5. Profitability Analysis

Analyzed:

- Profit by Category
- Profit by Region
- Sales vs Profit
- Profit Margin
- Product-level profitability
- Loss-making products

### 6. Customer Analysis

Analyzed:

- Customer-level sales
- Customer-level profit
- Customer order counts
- Customer segments
- Average Order Value (AOV)

### 7. Product Analysis

Analyzed:

- Top-selling products
- Most profitable products
- Loss-making products
- Product sales, profit, quantity, and profit margin

### 8. Discount Analysis

Investigated:

- Discount vs Profit
- Average profit by discount level
- Median profit by discount level
- Percentage of loss-making transactions by discount level

### 9. Correlation Analysis

Used:

- Correlation matrix
- Correlation heatmap
- Automated ranking of numerical correlation pairs

Correlation was used as a **screening tool for identifying potentially interesting relationships**, rather than as evidence of causation.

### 10. Operational Analysis

Analyzed:

- Shipping modes
- Number of orders by shipping mode
- Average shipping time
- Average shipping cost
- Total shipping cost

---

## 📈 Key Insights

### 1. Technology is a major revenue and profit driver

Technology is the highest-performing product category in terms of both total sales and total profit.

This indicates that Technology is an important contributor to the company's overall financial performance.

---

### 2. Central is the strongest region

Central is the leading region in both sales and profit.

This makes the region an important area for further investigation to understand its product mix, customer mix, and commercial performance.

---

### 3. Consumer is the largest revenue-generating segment

The Consumer segment contributes the highest sales among the customer segments.

Further analysis of order volume, customer count, average order value, and profitability can help explain why this segment performs strongly.

---

### 4. Sales show a strong upward trend

Sales increase across the observed years from 2011 through 2014.

This indicates strong historical revenue growth during the period covered by the dataset.

Year-over-year growth was also calculated to understand the rate of change rather than simply looking at the overall trend.

---

### 5. Higher discounts are associated with more loss-making transactions

The discount analysis indicates that higher discount levels are associated with a greater proportion of loss-making transactions.

This suggests that discount strategies should be evaluated together with their effect on profitability.

> **Important:** This analysis identifies an association, not proof that discounts directly cause losses.

---

### 6. High sales do not necessarily mean high profitability

The project compares sales, profit, and profit margin at the category and product levels.

This demonstrates why business decisions should not be based solely on revenue.

A product can generate substantial sales while still having weak or negative profitability.

---

### 7. Product-level analysis reveals additional opportunities

The analysis identifies both top-selling products and loss-making products.

This allows management to investigate whether factors such as discounts, shipping costs, regional demand, or product mix may be contributing to weak profitability.

---

## 💡 Business Recommendations

### 1. Protect high-performing categories

Investigate the factors contributing to Technology's strong sales and profitability.

This could include analyzing:

- Top-performing Technology products
- Regional demand
- Customer segments
- Discount levels
- Product margins

---

### 2. Learn from high-performing regions

Central is the strongest region in terms of sales and profit.

The company should investigate its product mix, customer composition, pricing, and discount patterns to determine whether successful practices can be applied to other regions.

---

### 3. Review high-discount transactions

High discount levels are associated with a greater percentage of loss-making transactions.

The company should evaluate whether the additional sales generated by high discounts justify the reduction in profitability.

---

### 4. Monitor products using both sales and profit

Products should not be evaluated using sales alone.

Management should monitor:

- Sales
- Profit
- Profit Margin
- Quantity
- Discount

This can help identify products that generate high revenue but weak profitability.

---

### 5. Use historical demand patterns for planning

The analysis identifies changes in sales over time and monthly sales patterns.

These trends can support:

- Inventory planning
- Marketing planning
- Promotional planning
- Demand forecasting

However, seasonal patterns should be validated across individual years before making major operational decisions.

---

## 📁 Project Structure

```text
Customer-Sales-Analysis/
│
├── data/
│   └── superstore.xls
│
├── notebooks/
│   └── Customer_Sales_Analysis_Portfolio.ipynb
│
├── images/
│   ├── sales_by_category.png
│   ├── sales_by_region.png
│   ├── sales_by_year.png
│   ├── monthly_sales.png
│   ├── top_products.png
│   ├── profit_by_category.png
│   ├── profit_by_region.png
│   ├── discount_vs_profit.png
│   └── correlation_heatmap.png
│
├── README.md
└── requirements.txt

# Sales Insight Dashboard – Power BI

## Overview
This project showcases end-to-end data analytics, including data cleaning, transformation, exploratory data analysis (EDA), KPI development, and dashboard visualization using Microsoft Power BI.

The final dashboard enables business teams to monitor performance, identify anomalies, and make data-driven decisions.

## Dataset
**Source:** `raw_data.xlsx`

**Includes:**
* Sales transactions
* Product information
* Customer & regional data
* Discount and profitability fields

Pre-processing steps include cleaning missing values, removing duplicates, standardizing formats, and building analytical tables.

## Data Preparation & Modeling
Key steps performed before visualization:

### Data Cleaning
* Handled missing values, inconsistent date formats, non-standard product categories
* Validated numeric fields (revenue, discount, profit)

### Data Transformation
* Created calculated columns for margin, profit %, discount tier
* Built star-schema style data model (Fact + Dimension tables)

### KPI Development (DAX)
Implemented DAX measures for:

* Total Revenue, Total Profit, Cost
* Average Discount %, Profit Margin
* YoY/ MoM growth
* Performance by Region, Product, Channel

## Dashboard Features
The interactive Power BI dashboard includes:

### 1. Executive KPI Summary
* Revenue, Profit, Margin, Discounts
* Real-time performance indicators
* Automatic refresh support

### 2. Sales Performance Analysis
* Regional comparison
* Product-level profitability
* Top/Bottom performing SKUs

### 3. Customer Insights
* Buying patterns
* Customer segments
* Repeat purchase behavior

### 4. Trend & Time Intelligence
* MoM / QoQ sales trends
* Forecasting using built-in analytics
* Anomaly detection on sales spikes/dips

## Key Insights Highlighted
* Region A contributes 42% of total revenue but shows declining MoM growth.
* Products in Category B have high volume but low margin, suggesting an optimization opportunity.
* Discount levels above 20% do not significantly increase sales volume → profit leakage risk.

## How to Use
1.  Clone/download the repository.
2.  Open the `.pbix` file using Power BI Desktop.
3.  Refresh data source if needed.
4.  Explore the dashboard through interactive filters and drill-downs.

## 🛠 Tools & Technologies
* Power BI Desktop
* DAX (for KPIs & measures)
* Excel / Power Query (data preparation)
* Data modeling (Star schema)
* Data cleaning & validation

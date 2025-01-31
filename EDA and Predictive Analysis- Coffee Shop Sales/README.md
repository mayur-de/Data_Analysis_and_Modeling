> # Exploratory and Predictive Analysis: Maven Roasters

> ## Project Overview

This project conducts an exploratory data analysis (EDA) of sales data from Maven Roasters, a coffee shop chain with three locations in New York City: Astoria, Hell's Kitchen, and Lower Manhattan. The goal is to uncover key insights about sales performance, customer behavior, and product trends to drive strategic decisions.

With over 149,000 transactions spanning six months, this analysis identifies **critical revenue drivers**, **high-value products**, and **temporal patterns** while offering **actionable recommendations to maximize profitability**.

> ## Objectives

The primary objectives of this project are:

- **Dataset Understanding**: Assess the structure, features, and completeness of the data.
- **Data Quality Checks**: Address missing data, outliers, and formatting issues.
- **Descriptive Analysis**: Summarize key performance indicators (KPIs) such as revenue, sales volume, and store performance.
- **Data Visualization**: Present insights visually for better communication of trends and patterns.
- **Relationship Analysis**: Identify correlations and patterns in customer purchases.
- **Advanced Analysis**: Explore advanced techniques such as predictive modeling.
- **Recommendations**: Make actionable recommendations based on the insights gained.

> ## Data Description

The dataset consists of transaction records from Maven Roasters' three stores. Key features include:

- `transaction_id`: A unique identifier for each transaction.
- `transaction_date`: The date of the transaction (MM/DD/YY).
- `transaction_time`: The timestamp of the transaction (HH:MM:SS).
- `transaction_qty`: The quantity of items sold.
- `store_id`: Unique ID of the coffee shop.
- `store_location`: Location of the coffee shop.
- `product_id`: Unique ID of the product sold.
- `unit_price`: Retail price of the product.
- `product_category`: Description of the product category.
- `product_type`: Description of the product type.
- `product_detail`: Description of the specific product.

The dataset contains 149,116 rows and 11 columns, covering a period of 181 days, from January 1, 2023, to June 30, 2023. There are 80 unique products, organized into 29 distinct product types and 9 product categories.

> ## Data Preprocessing

The following steps were taken to prepare the data for analysis:

- **Null Values and Duplicates**: Checked for null values and duplicate records. None were found.
- **Data Type Adjustments**: Adjusted data types for consistency and accuracy. For example, `transaction_date` was converted to datetime format.
- **Feature Engineering**:
  - **Date-Based Features**: Extracted variables such as `day_of_month`, `day_of_week`, and `month` from `transaction_date`.
  - **Time-Based Features**: Extracted the `hour` of the day from `transaction_time` to analyze sales patterns by time.
  - **Transaction Value**: Created a new feature, `transaction_value`, as the product of `transaction_qty` and `unit_price` to represent the sales amount.

> ## Key Findings

> ### Summary Metrics

- **Total Transactions**: 149,116.
- **Total Revenue**: $698,812.33.
- **Units Sold**: 214,470.
- **Average Daily Transactions**: 823.85 transactions per day.
- **Average Daily Revenue**: $3,860.84.
- **Revenue per Transaction**: $4.69.
- **Revenue per Unit Sold**: $3.26.
- **Increase in Monthly Revenue (Jan-June)**: 103.83%.
- **Increase in Transaction Frequency (Jan-June)**: 104.18%.

> ### Store Performance

- All three stores perform competitively, with **Hell's Kitchen** slightly leading in sales.

> ### Product Analysis

- **Coffee** dominates sales across all locations, contributing approximately 38% of total revenue.
- **Coffee and Tea** together account for about two-thirds of the total revenue.
- **Premium products** such as those in the **Coffee Beans** and **Branded** categories are typically higher priced.

> ### Transaction Patterns

- Transaction frequency increases from January to June.
- Peak transaction hours are between 8 AM and 11 AM.
- There is a noticeable drop in transactions after 5 PM.
- Weekends have lower transaction volumes than weekdays.
- **High-value transactions** make up a small percentage (2.19%) of total transactions but contribute 9.08% of the total sales.

> ### Key Relationships

- **Strong positive correlation (0.686)** between `unit_price` and `transaction_value`.
- **Weak to moderate positive correlation (0.356)** between `transaction_quantity` and `transaction_value`.
- **Weak negative correlation (-0.1235)** between `unit_price` and `transaction_quantity`.

> ## Recommendations

- **Focus on High-Value Products**: Prioritize Coffee Beans and Branded products, as they drive higher transaction values.
- **Optimize Staffing**: Ensure adequate staffing during peak hours (8 AM - 11 AM).
- **Targeted Promotions**: Consider promotions during midday dips (12 PM - 2 PM) and for lower-value items like bakery products.
- **Strategic Pricing**: Make strategic pricing adjustments for premium items.
- **Enhance Sales of Tea and Bakery**: Develop strategies to increase sales in the Tea and Bakery categories.
- **Leverage Location Strengths**: Tailor promotions to each location's unique sales trends, such as promoting Coffee Beans in Hell's Kitchen.
- **Data-Driven Decision Making**: Use heatmaps and line plots to track sales trends across the day.

> ## Repository Structure

```
├── Exploratory Data Analysis - Coffee Shop Sales
├── Predictive Analysis - Coffee Shop Sales
├── Executive Summary
├── README.md
```

> ## How to Use This Repository

1. Clone the repository to your local machine.
2. Navigate to the files.
3. Open and run the Jupyter Notebook files to reproduce the analysis and visualizations.
4. For predictive analysis, explore the `Predictive Analysis - Coffee Shop Sales.ipynb` notebook.

> ## Quick Start

1. Install Python 3.9+ and Jupyter Notebook.
2. Open and run `Exploratory Data Analysis - Coffee Shop Sales` to explore the EDA.
3. Open and run `Predictive Analysis - Coffee Shop Sales` for predictive analysis.

> ## Contributions

- If you have suggestions for improvement or find this project helpful, feel free to open an issue or fork the repository to contribute. 
- Feedback is always welcome!


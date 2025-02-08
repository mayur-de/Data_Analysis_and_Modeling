> # **Exploratory and Predictive Analysis: Maven Roasters**  

## **Project Overview**  
- **Goal**: Analyze sales data from Maven Roasters (Astoria, Hell’s Kitchen, Lower Manhattan) to uncover insights on revenue, customer behavior, and product trends.  
- **Scope**: 149,116 transactions over 181 days (Jan 1 – Jun 30, 2023).  
- **Focus**: `Revenue drivers`, `high-value products`, `temporal patterns`, and `actionable recommendations`.  

## **Objectives**  
1. **Dataset Understanding**: Assess structure, features, and completeness.
2. **Data Quality Checks**: Identify and handle missing data, outliers, and formatting issues.
3. **Descriptive Analysis**: Key KPIs (revenue, sales volume, store performance).
4. **Data Visualization**: Communicate trends effectively.
5. **Relationship Analysis**: Identify correlations in customer purchases.
6. **Advanced Analysis**: Explore predictive modeling.
7. **Recommendations**: Provide actionable insights.  

## **Data Description**  
- **149,116 rows, 11 columns** (Jan 1 – Jun 30, 2023).  
- **80 products** categorized into **29 product types and 9 product categories**.  
- **Key Features**:  
  1. `transaction_id`: A unique identifier for each transaction.
  2. `transaction_date`: The date of the transaction (MM/DD/YY).
  3. `transaction_time`: The timestamp of the transaction (HH:MM:SS).
  4. `transaction_qty`: The quantity of items sold.
  5. `store_id`: Unique ID of the coffee shop.
  6. `store_location`: Location of the coffee shop.
  7. `product_id`: Unique ID of the product sold.
  8. `unit_price`: Retail price of the product.
  9. `product_category`: Description of the product category.
  10. `product_type`: Description of the product type.
  11. `product_detail`: Description of the specific product.

## **Data Preprocessing**  
- **Null Values & Duplicates**: None found.  
- **Data Type Adjustments**: Converted `transaction_date` to datetime format.  
- **Feature Engineering**:  
  - Extracted **date-based features** (`day_of_month`, `day_of_week`, `month`).  
  - Extracted **time-based features** (`hour`).  
  - Created **`transaction_value`** (`transaction_qty × unit_price`).  

> # **Key Findings**  

### **Summary Metrics**  
- **Total Transactions**: 149,116  
- **Total Revenue**: $698,812.33  
- **Units Sold**: 214,470  
- **Avg. Daily Transactions**: 823.85  
- **Avg. Daily Revenue**: $3,860.84  
- **Revenue per Transaction**: $4.69  
- **Revenue per Unit**: $3.26  
- **Monthly Revenue Growth (Jan–Jun)**: +103.83%  
- **Transaction Frequency Growth (Jan–Jun)**: +104.18%  

### **Store Performance**  
- All stores perform competitively, with **Hell’s Kitchen leading in sales**.  

### **Product Analysis**  
- **Coffee**: Dominates sales (38% of total revenue).  
- **Coffee & Tea**: ~66% of total revenue.  
- **Premium Products (Coffee Beans, Branded items)**: Higher price points.  

### **Transaction Patterns**  
- **Increasing transaction frequency** (Jan–Jun).  
- **Peak sales hours**: 8 AM – 11 AM.  
- **Sales drop after 5 PM**.  
- **Weekends**: Lower transaction volume.  
- **High-value transactions (2.19%)** contribute **9.08%** of total sales.  

### **Key Relationships**  
- **Strong correlation (0.686)**: `unit_price` & `transaction_value`.  
- **Moderate correlation (0.356)**: `transaction_qty` & `transaction_value`.  
- **Weak negative correlation (-0.1235)**: `unit_price` & `transaction_qty`.  

## **Recommendations**  
- **Focus on High-Value Products**: Prioritize **Coffee Beans & Branded products**.  
- **Optimize Staffing**: Increase staff during **peak hours (8 AM – 11 AM)**.  
- **Targeted Promotions**: Offer deals during **midday dips (12 PM – 2 PM)**.  
- **Strategic Pricing**: Adjust premium item prices.  
- **Boost Tea & Bakery Sales**: Implement marketing strategies.  
- **Leverage Store Strengths**: Tailor promotions based on location trends.  
- **Data-Driven Decision Making**: Use **heatmaps & line plots** for tracking sales trends.  
---
## **Repository Structure**  
```
├── Exploratory Data Analysis - Coffee Shop Sales
├── Predictive Analysis - Coffee Shop Sales
├── Executive Summary
├── README.md
```

## **How to Use This Repository**  
1. Clone the repository.  
2. Open files and run Jupyter Notebooks.  
3. Explore `Predictive Analysis - Coffee Shop Sales.ipynb` for forecasting insights.  

## **Quick Start**  
1. Install Python 3.9+ & Jupyter Notebook.  
2. Run `Exploratory Data Analysis - Coffee Shop Sales.ipynb`.  
3. Run `Predictive Analysis - Coffee Shop Sales.ipynb` for predictions.  

## **Contributions**  
- Open issues or fork the repository for improvements.  
- Feedback is welcome! 

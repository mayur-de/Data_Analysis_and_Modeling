> # **Cost and Profit Analysis: Food Delivery Platform**

> ## 📌**Project Overview**
This project analyzes the financial and operational aspects of a food delivery platform to:
- **Assess the cost structure.**
- **Identify inefficiencies.**
- **Recommend strategies to enhance profitability.**

By analyzing transactional data, the project:
- **Identifies key cost drivers.**
- **Quantifies revenue performance.**
- **Provides actionable recommendations to optimize operations and improve net income.**

> ## 💡**Recommendations for Platform to Increase Profitability**
1. **Reduce Discounts**: Discounts constitute nearly half of the total costs.
2. **Increase Commission Fees**: Strong correlation with net income.
3. **Optimize Refund Rates**: High refund rates negatively impact profitability.
4. **Encourage Larger Order Values**: Larger orders positively influence net income.
5. **Revise Delivery Fee Structure**: Reassess fee coverage to minimize cost burdens.
6. **Minimize Processing Fees**: Optimize payment gateway agreements.

> ## 📊**Data Description**
The dataset consists of transactional records for 1,000 orders from the food delivery platform, covering essential financial and operational metrics.

> ### ***Key Features:***
- **Order Details** – Unique identifiers, timestamps, customer/restaurant information.  
- **Financial Metrics** – Order value, delivery fees, discounts, refunds.  
- **Revenue Sources** – Commission fees and payment details.  

| Column Name               | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| Order ID                 | Unique identifier for each order                                           |
| Customer ID              | Unique identifier for the customer placing the order                       |
| Restaurant ID            | Unique identifier for the restaurant fulfilling the order                  |
| Order Date and Time      | Date and time when the order was placed                                    |
| Delivery Date and Time   | Date and time when the order was delivered                                 |
| Order Value              | Total value of the food items in the order (before fees and discounts)     |
| Delivery Fee             | Fee charged for delivering the order (cost to the platform)               |
| Payment Method           | Mode of payment used by the customer                                      |
| Discounts and Offers     | Discounts or promotional offers applied to the order                      |
| Commission Fee           | Fee charged by the platform for facilitating the order (revenue source)   |
| Payment Processing Fee   | Fee charged by the payment gateway for processing payments (cost)         |
| Refunds/Chargebacks      | Amount refunded or charged back due to disputes or cancellations (cost)   |

> ## 🏗 **Feature Engineering**  
- **Discount Percentage (Disc Pct)** – Extracted from 'Discounts and Offers'.  
- **Discount Amount** – Calculated as discount percentage × order value.  
- **Cost** – Summed: **Delivery Fee + Discount Amount + Payment Processing Fee + Refunds/Chargebacks** 
- **Revenue** – Defined as 'Commission Fee'.  
- **Net Income** – Revenue minus Cost.  
- **Date** – Extracted from 'Order Date and Time'.

> ## 🔍**Key Findings**
> ### **Financial Performance**
- **Total Loss**: ₹34,051.85.
- **Revenue-to-Cost Ratio**: 0.79 (₹0.79 earned for every ₹1 spent).
- **Average Cost per Order**: ₹161.04, while revenue per order is ₹126.99.
- **Net-Income-to-Revenue Ratio**: -0.27, indicating 27% of revenue is insufficient to cover costs.
- **Revenue Share**: Revenue constitutes only 12% of the average order value.

> ### **Cost Drivers**
- Discounts account for **46.13%** of total costs, averaging ₹74.29 per order.
- Refund rate is **28.5%**, significantly impacting operational efficiency.
- Delivery fees impact **81.4%** of orders.

> ### **Profitability Insights**
- **61.8%** of orders are loss-making, while **37.9%** are profitable.
- Profit-making orders feature lower discounts, fewer refunds, and higher commission fees.

> ## 📂 **Repository Structure**  
```
│
├── Cost and Profit Analysis - Food Delivery Platform.ipynb
├── Executive Summary.pdf
├── README.md
```
> ## 🚀 **How to Use This Repository**  
1. Clone the repository to your local machine.  
2. Navigate to the files and open Jupyter Notebook.
3. Open `Cost and Profit Analysis - Food Delivery Platform.ipynb` for a detailed breakdown of costs and revenue.  

> ## ⚡ **Quick Start**  
1. Install **Python 3.9+** and **Jupyter Notebook**.
2. Run `Cost and Profit Analysis - Food Delivery Platform.ipynb` to explore insights.  

> ## 🤝 **Contributions**  
If you have suggestions for improvement or find this project helpful:  
- Open an **issue**.  
- Fork the repository to **contribute**.  
- Feedback is always welcome! 

---
> ## ✍️ **Author**  
- **Mayurkumar Deshmukh**  
- 📧 [mayurkumar.de@gmail.com]  
- 🌐 [LinkedIn Profile](https://www.linkedin.com/in/mayurkumar-deshmukh/)  

---- **_Happy Analyzing!!!_** ----

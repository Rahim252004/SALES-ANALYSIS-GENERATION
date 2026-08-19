# Sales Data Analysis 📊

## Project Overview
This project analyzes 2024 sales data to uncover patterns in product performance, regional performance, monthly trends, and customer behavior. The goal is to answer key business questions and provide actionable recommendations.

## Dataset
- **Rows:** 1,015 raw orders (1,000 unique orders after cleaning)
- **Columns:** order_id, date, product, region, quantity, unit_price, customer_id, total_sales
- **Time period:** January – December 2024
- **Total revenue (after cleaning):** $1,906,135
- **Total units sold:** 4,974

## Data Cleaning
- Handled missing values in `product` (filled with "Unknown") and `unit_price` (filled using the average price per product)
- Removed duplicate order rows
- Standardized inconsistent region names (e.g. "north" vs "North")
- Verified `total_sales` consistency against `quantity × unit_price`

## Exploratory Data Analysis
Analysis covered:
- Revenue by product
- Revenue by region
- Monthly revenue trends
- Top customers by revenue contribution

## Key Findings
- 🏆 **Laptop** is the highest-revenue product (~$408,795), followed by Phone and Tablet
- 🌍 **North** is the strongest region, generating ~$754,680 (~40% of total revenue)
- 📅 **May** recorded the highest monthly revenue, while **March** recorded the lowest — indicating noticeable seasonal fluctuation
- Data quality issue: a portion of orders had missing product information (now labeled "Unknown")

## Business Recommendations
1. **Focus on high-performing products** — maintain strong inventory and marketing for Laptop, Phone, and Tablet
2. **Strengthen weaker regions** — investigate demand, marketing reach, and product preferences in lower-performing regions
3. **Improve data collection** — reduce "Unknown" product entries by fixing data capture at the point of sale
4. **Monitor monthly fluctuations** — align inventory and marketing planning with seasonal peaks and declines

## Conclusion
This project analyzed 2024 sales data to identify sales patterns, product performance, regional performance, customer behavior, and monthly trends. After cleaning (missing values, duplicates, inconsistent region names, and sales calculation checks), the dataset contained 1,000 unique orders generating $1,906,135 in total revenue from 4,974 units sold. Laptop was the strongest product by revenue, North was the strongest region, and monthly analysis revealed clear seasonal fluctuation. These findings support decisions in inventory management, regional marketing, product strategy, and customer retention.

## Technologies Used
Python, Pandas, NumPy, Matplotlib/Seaborn, Jupyter Notebook

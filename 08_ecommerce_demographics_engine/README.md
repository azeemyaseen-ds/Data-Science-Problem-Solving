# Case File 8: E-Commerce Demographics Engine
**Domain:** Advanced Retail Analytics & Pricing Strategy

# Business Problem:
An e-commerce compamy operating across different cities uploaded an messy, unaggregated transaction ledger. The regional marketing team wants to identify geographical spending behavious to adjust shipping fees, but they need to flag revenue anomalies (outliers).

# Technical Approach:
 * Create `Total_Revenue` column by multiplying `Units_Sold * Unit_Price_PKR`.
 * Use `groupby() & agg()` methods to calculate `total_revenue` and `avg_units_sold` by each city.
 * Calculate `avg_transaction_revenue` by using the built-in `mean()` function.
 * Use conditional operators (>) to **filter** the dataframe.
 * Use `groupby()` method to calculate revenue by each category. Then calculate the **market share percentage** of each product category in a total business transaction revenue.
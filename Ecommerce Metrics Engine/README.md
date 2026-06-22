# Case File 3: The E-Commerce Metrics Engine
**Domain:** Business Intelligence & E-Commerce Analytics

# Business Problem:
An online shopping platform wants to launch a mid-year dashboard. The database delivers daily sales records as a list of dictionaries. But before updating the business wants that the data analyst can figure out the average order value (AOV) and best performing product categories by revenue.

# Technical Approach:
 * Use `Revenue = Price * Quantity` to calculate the revenue by each order to calculate the total revenue of the entire platform.
 * Use dictionary to calculate product by revenue to figure out the best performing product categories.
 * Use `Average Order Value (AOV) = Total Revenue / Total no. of Orders` to calculate how much each customer spend while placing
a single order.
 * Structured the code into a reusable function adhering the DRY principle.
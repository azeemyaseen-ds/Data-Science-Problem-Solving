# Case File 9: Islamabad Telecom Churn
**Domain:** Subscription Analytics & Revenue Assurance

# Business Problem:
A broadband service provider import dirty customer health dataset. The dataset contain missing values, mismatched text, and raw financial columns. The product team needs an priortize outreach sheet consisting of high value users at immediate risk of leaving the network (churning) so the account manager can call them today.

# Technical Approach:
 * Use `.astype(float)` to convert the `Monthly_Bill_PKR` column from string to numeric.
 * Use `.str.strip()` to remove the trailing spaces of the values of `Package` column.
 * Use `.fillna()` to replace the missing values of the `Data_Usage_GB` column.
 * Apply 3 conditions on different columns to **figure the high value users at immediate risk of leaving the network**. So the business can **retain their high value users**.
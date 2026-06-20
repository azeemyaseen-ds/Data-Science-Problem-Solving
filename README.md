# Case File 2: The Duplicate Loyality Fraud Detection
**Domain:** Retail Analytics & Customer Relationship Management (CRM)

# Business Problem:
The retail chain launched a Loyalty Card Program. Customers earn points every time they shop. However the data engineering team figureout the bug on mobile app: some users are register multiple times using slight variations of their names and phone numbers to exploit the system and claim duplicate welcome rewards.
The regional manager needs a automated fraud-detection script to clean the data and flag suspicious users before the weekly rewards are distributed.

# Technical Approach:
 * Normalized the Data using` lower(), join(), strip(), split(), replace()` to clean the messy data to figured out the **suspicious accounts**.
 * Use tracking `set()` to separate **valid** users and **duplicate** users.
 * Use the normalize records to check if this record uses a name or phone that flag as duplicate to **LOCK ACCOUNT**.
 * Calculate the **Total Frozen Points** belong to suspicious accounts to take them under Investigation.
# Case File 4: The Server Log Error Miner
**Domain:** DevOps & Data Infrastructure Engineering

# Business Problem:
The engineering team experience a brief system slow down. Their Server generated raw text log file containing system status reports. The infrastructure manager needs summary report of how many **ERROR messages** occured and which system is failing the most so they can deploy a bug fix.

# Technical Approach:
 * Split the raw string into 3 clean parts using intentional delimeter.
 * Extract the log level & module name using python indexing.
 * Only focus on ERROR messages using if condition and calculate how many errors occured in the whole system.
 * Use dictionary to calculate ERROR messages by specific module. So the business can figure which system is failing the most and deploy a bug fix.
# Case File 5: The Islamabad Tech Talent Pool Analytics
**Domain:** HR Analytcis & Workforce Planning

# Business Problem:
 - The Company wants to analyze their applicants pool for an upcoming internship cycle. They recieve hundreds of short applicants profile but their HR Database glitched, and their raw data was saved as a single list of string.
 - The HR Directors wants an automated talent analytics function that evaluates how many customers are from different cities, who has the required skills, and the average test scores of applicants to plan their hiring budget.

# Technical Approach:
 * Split the string using a intentional delimeter.
 * Use Dictionary comprehension to create key value pairs using split parts & also remove the extra spaces around the words.
 * Use if condition to identify the applicants from **Islamabad** with having **Python**.
 * Use dictionary to figure out how many customers from each city.
# Case File 7: The Islamabad Salary & Remote Work Analyzer
**Domain:** HR Tech & Labor Market Analytics

# Business Problem:
A tech association conduct a survey of software developers across Pakistan to understand the local compensation structures. They want to identify the highest paid remote workers living in Islamabad to set salary benchmark for upcoming tech startups.

# Technical Approach:
 * Convert the dictionary of lists into a pandas dataframe to perform vectorized operations on data using `pd.DataFrame`.
 * Use the `.info()` method to get the concise summary of the dataframe.
 * Use `df[(df['col'] == 'value')]` to filter the dataframe.
 * Use `.idxmax()` to figure out the index of maximum values.
 * Use `.loc` extract the employee name using the index their highest salaries.
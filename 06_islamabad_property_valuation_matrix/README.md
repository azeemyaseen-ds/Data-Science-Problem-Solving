# Case File 6: The Islamabad Property Valuation Matrix
**Domain:** Real Estate & Property Tech

# Business Problem:
A real estate investement company is evaluating residential plots. Instead of checking prices manually, they want an **algorithm to compute estimated property values** based on total squared footage and price per square foot, adjusted for tax prices.

# Technical Approach:
 * Calculate the **base price** of the plot by multiplying `total squared footage * price per square foot` using **vectorization**.
 * Calculate the **final price** of plot by multiplying `base price * sector premimum` using **vectorization**.
 * Format the output of an array using `np.set_printoptions()`.
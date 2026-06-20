# Case File 1: The Corrupted Logistic Logs
**Domain:** Supply Chain & E-commerce Logistics

# Business Problem
An automated logistics system generated a batch report with corrupted data types (string representation of floats) and negative values due to sensor malfunction.

# Technical Approach
 * Implemented a strided loop (`range(0, N, 3)`) to parse sequential chunk data.
 * Handled type casting dynamically using Python built-ins.
 * Applied absolute value corection (`abs()`) to troubleshoot data anomalies without losing tracking records.
 * Structured the final code into a reusable function adhering to DRY principles.
# Case File 10: The Islamabad Tech Hub Energy Grid Anomaly Matrix
**Domain:** City Infrastructure & Operations Analytics

# Business Problem:
A smart city tech park complex tracks electricity consumption across multiple operational wings (data centers, software labs, incubators). The lot meter generated raw log dataset containing timestamps, raw power metrics, and operational flags. The facility engineer wants an automated warning system that flag the wings that use way too much electricity or way too little electricity compare to what they normally use.

# Technical Approach:
 * Use `pd.to_datetime()` method to convert the `Reading_Time` string column into a datetime column.
 * Use `td.hour` to extract the hour from the `Reading_Time` datetime column to create a standalone column named `Hour`.
 * Use `groupby()` method to group data by `Facility_Wing` then apply `agg()` to create a summary table by performing mathematical operations on the data.
 * Use `mean()` and `std()` built-in methods to calculate mean and standard deviations to further calculate the upper and lower limits to identify outliers.
 * Use (`|`) operator in conditions to filter outliers to warn the facility engineer immediately.
 * Also identified the **risk periods** for the facility engineer.
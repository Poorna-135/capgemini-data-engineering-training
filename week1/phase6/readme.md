Phase 6 – Spark Playground Exit Sprint (Advanced Practice Lab)
🔹 Objective

In this phase, the goal is to build fluency and confidence in PySpark by solving advanced problems involving joins, window functions, date operations, and complete pipeline execution.
---

🔹 Problem Summary

We were given dirty datasets (customers and orders) containing:

• Null values

• Invalid records (negative amounts, wrong foreign keys)

• Duplicates

The task was to:

• Clean and validate the data

• Perform joins between datasets

• Apply aggregations and window functions

• Build a complete data pipeline
---
🔹 Approach

Loaded datasets into PySpark DataFrames

Performed data cleaning:

o Removed null values in important columns

o Filtered invalid records (negative amounts)

o Trimmed string columns

o Removed duplicate records

Validated data integrity:

o Used left_anti join to identify invalid foreign keys

Joined datasets using appropriate join types:

o Inner join for valid records

o Left join for validation

Applied transformations:

o groupBy and aggregations (total spend, order count)

o Filtering invalid records

Applied window functions:

o Ranking customers by total spend

o Running totals and lag operations

Performed date-based analysis:

o Extracted month from date

o Aggregated monthly sales

Saved final output dataset
---
🔹 Key Transformations Used

• join() → to combine customers and orders

• left_anti join → to detect invalid foreign keys

• groupBy() → for aggregations

• agg() → to calculate sum, count

• filter() → to remove invalid data

• dropna() → to handle null values

• dropDuplicates() → to remove duplicate records

• Window functions → for ranking and analysis

• to_date(), month() → for date operations
---
🔹 Output / Results

The following outputs were generated:

• Cleaned datasets (customers and orders)

• Validated dataset (invalid foreign keys identified)

• Aggregated customer-level metrics (total spend, order count)

• Ranked customers based on spending

• Monthly sales analysis
---
🔹 Data Engineering Considerations


• Ensured data cleaning before transformations

• Validated referential integrity using joins

• Avoided duplicate records after joins

• Handled null and invalid values carefully

• Verified outputs using counts and sample checks

---
🔹 Challenges Faced

• Identifying invalid foreign keys using joins

• Handling dirty data (nulls, गलत values)

• Understanding window functions

• Managing multiple transformations in a pipeline

---
🔹 Learnings

• Advanced joins (inner, left, left_anti)

• Importance of data validation in pipelines

• Use of window functions for analytics

• Handling real-world dirty datasets
• Building end-to-end PySpark pipelines

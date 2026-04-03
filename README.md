This repository contains all the things we've learned in the data training.

WEEK 0:

--->Phase 0:

   Completed the Databricks Associate Data Engineering course
    
--->Phase 1:

📚Topics covered: SELECT, FILTER, GROUP BY

✅Key learnings: Understanding GROUP BY and its applications 
               SQL to PySpark mapping
              
⚠️Challenges faced :Grasping the concept of GROUP BY 
                  Writing joins in pyspark

--->Phase 2:


📚 Topics Covered:
Joins and aggregations in PySpark, mapping SQL queries to DataFrame operations.

✅ Key Learnings:
Learned to use join(), groupBy(), sum(), avg(), filter(), and orderBy(), and understood how SQL logic translates to PySpark.

⚠️ Challenges:
Faced difficulty with writing correct join conditions, understanding join types, and applying multiple aggregations together


--->Phase 3:


📚 Topics Covered:
ETL pipeline (Extract → Transform → Load), data ingestion from CSV files, data cleaning (null handling), schema validation, joins, aggregations, and pipeline-based transformations in PySpark.

✅ Key Learnings:
Learned how to read and process real-world data, handle missing values using dropna() and fillna(), convert data types using cast(), and build a structured pipeline using join(), groupBy(), sum(), count(), and window functions. Also understood how to move from SQL queries to end-to-end PySpark workflows.

⚠️ Challenges:
Faced issues with null values, incorrect data types (string to numeric), writing proper join conditions, and understanding the correct order of operations in an ETL pipeline.

---> Phase 4:

📚 Topics Covered: End-to-end data pipeline creation, data cleaning (null removal, duplicates, invalid values), joins between datasets, aggregations, customer segmentation, and final reporting using PySpark.
4A: different bucketing techniques

✅ Key Learnings: Learned how to build a complete business pipeline from raw data to insights, perform data cleaning before processing, calculate metrics like daily sales, city-wise revenue, and customer spend, and apply business logic for segmentation (Gold, Silver, Bronze). Also understood how to combine multiple transformations into a final reporting table and save outputs. and also ddid it using multiple bucketing/segmentation methods

⚠️ Challenges: Faced issues with handling null keys before joins, deciding correct join order, managing duplicates and invalid data, writing aggregation logic for multiple tasks, and combining all outputs into a single final dataset.

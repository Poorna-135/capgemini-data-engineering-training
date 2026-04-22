Raw Data Ingestion (Telecom Dataset)

🔹 Objective

The objective of this phase is to ingest raw telecom data into a cloud-based storage system and make it available for further processing.
This includes setting up storage, loading data, and establishing connectivity with the processing platform.

🔹 Problem Summary

Telecom organizations generate large volumes of data across multiple domains such as customers, usage, subscriptions, and complaints.

The challenge is to:

Collect data from different sources
Store it in a centralized and scalable system
Ensure accessibility for downstream processing

🔹 Dataset Overview

The dataset consists of 8 tables representing different aspects of telecom operations:

campaigns → Marketing campaign details
complaints → Customer complaints and issues
customers → Customer demographic and account information
plans → Subscription plans and pricing
recharges → Recharge and payment transactions
subscriptions → Customer subscription details
towers → Network tower information
usage → Customer usage data (calls, data consumption, etc.)

This dataset provides a complete view of telecom business operations.

🔹 Approach

Provisioned cloud storage using an Amazon S3 bucket
Ingested raw telecom data into the storage bucket
Organized data into appropriate folders for each table
Connected the storage system to Databricks using an external connector
Verified data accessibility for further processing

🔹 Technologies Used

Amazon Web Services (S3) – Cloud storage for raw data
Databricks – Data processing and analytics
External Connector – To establish secure connection between storage and Databricks

🔹 Implementation Details

1. Storage Setup
Created an S3 bucket using a stack
Uploaded telecom dataset files into the bucket
Structured data into folders for better organization
2. Data Ingestion
Loaded all 8 tables into the S3 bucket
Ensured data is stored in raw format without modifications
3. Connectivity
Connected S3 to Databricks using external connector
Configured access permissions
Verified successful data access from Databricks

🔹 Key Features

Centralized storage of raw telecom data
Scalable cloud-based storage system
Secure connectivity between storage and processing platform
Organized dataset for easy access and processing

🔹 Output / Results

Successfully ingested all 8 telecom tables into S3
Established connection with Databricks
Data is available for further transformation and analysis

🔹 Data Engineering Considerations

Maintained raw data without transformations
Ensured proper folder structure for each table
Configured secure access between S3 and Databricks
Designed storage for scalability and future growth

🔹 Challenges Faced

Setting up S3 bucket using stack configuration
Configuring secure access between S3 and Databricks
Ensuring correct data paths and connectivity
Managing multiple datasets efficiently

🔹 Learnings

Basics of cloud data storage using S3
How to ingest and organize raw data
Connecting external storage to Databricks
Importance of centralized data storage in data engineering

🔹 Conclusion

This phase establishes the foundation of the data pipeline by ingesting raw telecom data into a scalable cloud storage system.
It ensures that all data is centrally available and ready for further processing and transformation.

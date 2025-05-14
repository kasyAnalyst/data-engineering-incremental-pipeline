
### Incremental Change Data Capture Pipeline on AWS
##

**Technology used:** Python, AWS Glue, AWS Step Functions, AWS Lambda, AWS DMS, Amazon Redshift, Amazon S3, VPC, AWS CloudFormation, AWS QuickSight

### Abstract
##
This project is an end-to-end data engineering pipeline built to handle **incremental processing of change data** from an operational database using the **Change Data Capture (CDC)** pattern. The primary goal is to build a scalable, automated pipeline that captures data changes and delivers them to an analytics-ready **Redshift** warehouse. This setup supports efficient, near real-time updates and minimizes system load.


### Process
##
* Started with **AWS CloudFormation** to provision necessary resources (VPC, IAM roles, etc.)
* Used **AWS DMS** to capture full and ongoing changes from the source database
* Stored raw and transformed data in **Amazon S3** buckets
* Created transformation jobs in **AWS Glue** using PySpark
* Orchestrated the entire workflow using **AWS Step Functions** to sequence and manage tasks like data extraction, transformation, and loading (ETL)
* Leveraged **AWS Lambda** for custom functions and automation within the pipeline
* Loaded curated datasets into **Amazon Redshift** for analytics

### Source code:
##
* ETL scripts and Glue job code
* CloudFormation templates
* Lambda functions for pipeline orchestration
* Configuration files for DMS and Redshift

### Output
##
* Visualized the final transformed data using **AWS QuickSight** for generating dashboards and reports
* Enabled interactive data exploration for actionable insights from the processed data in **Amazon Redshift**
* [View Dasboard](https://drive.google.com/file/d/1ls5qioUdlYjd_Z1LnyVEyHbSm9Laymit/view?usp=sharing)



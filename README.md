# Redfin Real Estate Data Analytics ETL Project

## Overview
This project focuses on extracting real estate data from the Redfin data center, transforming it using Python and Apache Airflow, and finally loading the processed data into Snowflake data warehouse for analysis. The entire ETL (Extract, Transform, Load) process is orchestrated and automated using Apache Airflow, with data transformation accomplished using pandas. Moreover, Snowpipe is employed to facilitate the seamless transfer of data from Amazon S3 to Snowflake. Additionally, Tableau is harnessed for data visualization purposes, accessible through the following link: [Tableau Redfin Real Estate Analytics Dashboard](https://public.tableau.com/views/Redfin_Real_Estate_Analytics/Dashboard1?:language=en-GB&:display_count=n&:origin=viz_share_link)




## Technologies Used
- Apache Airflow: An open-source platform for orchestrating and scheduling workflows, Apache Airflow is used to automate and manage the end-to-end ETL process.

- Snowpipe: This Snowflake feature automates the data loading process, ensuring that as soon as data lands in an Amazon S3 bucket, it is loaded into a Snowflake data warehouse table.

- Snowflake: A cloud-based data warehousing platform that enables efficient storage and analysis of large datasets.

- AWS Services: Amazon S3 is utilized as the storage solution for both raw and transformed data.

- Python: The ETL process involves extracting data from the Redfin data center using Python, with pandas employed for data transformation.

- Tableau: After loading the data into Snowflake, Tableau is connected to the Snowflake data warehouse to visualize and gain insights from the real estate data.

## Project Structure
- Data Extraction:
Python scripts are employed to connect to the Redfin data center data source and extract real estate data.

- Data Transformation:
Pandas is used for data transformation, ensuring the extracted data is formatted and processed appropriately.

- Data Loading:
The transformed data is loaded into an Amazon S3 bucket, and raw data is also stored in a separate S3 bucket.

- Snowflake Integration:
Snowpipe is triggered as soon as transformed data lands in the AWS S3 bucket, automatically executing a COPY command to load data into a Snowflake data warehouse table.

- Workflow Orchestration:
Apache Airflow orchestrates and automates the entire ETL process, ensuring seamless execution and scheduling of tasks.

- Visualization:
Tableau is connected to the Snowflake data warehouse, enabling the creation of insightful visualizations for data analysis.


## Setup Instructions
To set up and run this project, follow these steps:

1. Install Dependencies:
Install Apache Airflow on your EC2 instance.

2. Configure AWS Credentials:
Set up AWS credentials to enable access to S3 buckets.

3. Redfin Data Extraction:
Implement Python scripts to connect to the Redfin data center and extract real estate data.

4. Data Transformation:
Utilize pandas for data transformation, ensuring proper formatting and cleaning.

6. Amazon S3 Configuration:
Configure Amazon S3 buckets for both raw and transformed data.

7. Snowflake Integration:
Set up Snowflake and configure Snowpipe to automatically load transformed data into the data warehouse.

8. Apache Airflow Configuration:
Configure Apache Airflow DAGs to orchestrate and automate the ETL workflow.

9. Run the ETL Process:
Trigger the Apache Airflow DAG to initiate the ETL process.

10. Tableau Connection:
Connect Tableau to the Snowflake data warehouse for data visualization.


## Conclusion
This Redfin Real Estate Data Analytics project demonstrates an end-to-end ETL process, showcasing the seamless integration of various technologies to extract, transform, and load real estate data for analysis.

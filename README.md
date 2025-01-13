
# ETL Automation Using Python, MySQL and Apache Airflow
This project demonstrates an automated ETL (Extract, Transform, Load) pipeline to process and analyze employee data. The pipeline uses Python, MySQL, and Apache Airflow for data processing, workflow orchestration, and scheduling.

# Overview
The ETL pipeline automates the extraction of data from a MySQL database, filters employees older than 30 years, and schedules periodic execution using Apache Airflow.

# Features
* **Database Integration :** Data storage and querying with MySQL.
* **ETL Automation :** Python script to extract and transform data.
* **Workflow Scheduling :** Apache Airflow DAG for scheduling and monitoring.
* **Error-Free File Handling :** Timestamped file names to avoid duplication.
* **Linux Compatibility :** Deployable on Ubuntu for efficient task execution.

# Project Workflow
**1. Database Setup**<br>
Create a MySQL database and populate it with employee records.

**2. Python ETL Script**<br>
Extracts employee data with age > 30 years.<br>
Flexible SQL queries for other use cases.

**3. Apache Airflow**<br>
DAG (etl_dag.py) schedules ETL every 10 minutes.<br>
Orchestrates the execution of the ETL process.

**4. Wrapper Script**<br>
wrapper_script.sh runs the Python ETL script.<br>
Invoked by Airflow DAG to ensure seamless execution.

**5. Error Handling**<br>
Unique filenames generated with timestamps to prevent errors.

# Technologies Used
* Python
* MySQL
* Apache Airflow
* Linux Ubuntu

# How to Run the Project
Set up the MySQL database and add sample employee data.
Configure the ETL script (etl_script.py) with the necessary queries.
Set up Apache Airflow and define the DAG file (etl_dag.py).
Ensure the wrapper script (wrapper_script.sh) is placed in the correct Ubuntu directory.
Use Airflow's scheduling to run the pipeline every 10 minutes.

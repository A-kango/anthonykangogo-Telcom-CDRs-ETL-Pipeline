
# 📞 Telcom CDRs ETL Pipeline

This project implements an ETL (Extract, Transform, Load) pipeline that processes telecom Call Detail Records (CDRs). The pipeline extracts raw call log data from a **MySQL** database, transforms it using **Pandas**, and loads the clean data into a **PostgreSQL** data warehouse. The pipeline is designed to support reporting and dashboarding in **Power BI**.

> Built with Python for practical data engineering workflows.

## 🔄 ETL Workflow

MySQL (Raw CDRs)  
↓  
Pandas (Clean & transform)  
↓  
PostgreSQL (Data warehouse)  
↓  
Power BI (Dashboards & Analysis)

## 📌 Features

- Extracts CDR data from MySQL using SQLAlchemy
- Cleans, sorts, removes duplicates, and fills missing values using Pandas
- Loads the transformed dataset into a PostgreSQL data warehouse
- Ready for visualization in Power BI
- Extendable with Apache Airflow for automation

## 🛠️ Technologies Used

- Python 3.10+
- Pandas
- SQLAlchemy
- MySQL Connector
- PostgreSQL
- Power BI


## 🚀 How to Run the Script

1. Ensure MySQL and PostgreSQL servers are running
2. Update the credentials in `etl_script.py` if needed
3. Run the ETL script using:


Expected Output:

Data loaded successfully into PostgreSQL.
ETL process completed.

## 🧱 Example PostgreSQL Schema

```sql
CREATE TABLE call_logs (
    caller_number VARCHAR,
    receiver_number VARCHAR,
    call_duration INT,
    call_time TIMESTAMP,
    caller_location VARCHAR,
    receiver_location VARCHAR
);

👤 Author
Engineer Anthony Kangogo
GitHub Profile


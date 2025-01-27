# kafka-stock-market-aws-project
## Project Overview
This project demonstrates an End-to-End Data Engineering solution for processing and analyzing real-time stock market data using Apache Kafka and AWS services. The goal of this project was to ingest, store, and process large-scale stock market data with a focus on scalability and reliability, leveraging key technologies such as Python, AWS (EC2, Glue, Athena), and Apache Kafka.

## Technologies Used
### Apache Kafka: For building a distributed messaging system, handling real-time streaming data.
- **Apache Kafka**: For distributed streaming of real-time data.
- **Python**: For developing the Kafka Producer and Consumer, as well as automating data tasks.
- **AWS**:
  - **EC2**: For hosting Kafka and Zookeeper.
  - **S3**: For storing real-time data.
  - **Glue**: For data cataloging and ETL tasks.
  - **Athena**: For querying the stock market data stored in S3.
  - **IAM**: For securely interacting with AWS services.
 
    ## Workflow

1. **Kafka Setup**:
   - EC2 instance launched and Kafka + Zookeeper installed.
   - Kafka **Producer** and **Consumer** configured to stream stock market data in real-time.

2. **Data Ingestion**:
   - Python scripts developed to send stock market data to Kafka and retrieve data with Kafka **Consumer**.

3. **AWS Integration**:
   - Data stored in an **S3 bucket**.
   - **IAM roles** created for secure interaction with AWS.
   - **AWS Glue Crawlers** configured for data cataloging.
   - **AWS Athena** used to query and view real-time data.

## Features

- Real-time stock market data streaming via Kafka.
- AWS integration for secure and scalable data storage and querying.
- Easy querying of data using SQL with Athena.

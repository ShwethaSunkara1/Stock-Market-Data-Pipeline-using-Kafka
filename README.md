# Stock-Market-Data-Pipeline-using-Kafka
This project simulates real-time stock market data streaming using Apache Kafka and processes it end-to-end with AWS services. A Python-based Kafka producer ingests data from a CSV dataset and streams it to a Kafka broker hosted on Amazon EC2. A Kafka consumer listens to this stream and writes the data to Amazon S3, which is then cataloged using AWS Glue and queried using Amazon Athena.

![Architecture](https://github.com/user-attachments/assets/8ccaf124-ccc8-46cc-9372-73ea1527e3cb)


🔧 Tech Stack
Apache Kafka (hosted on Amazon EC2)

Python (kafka-python, boto3, pandas)

Amazon S3 for data storage

AWS Glue for cataloging

Amazon Athena for SQL-based querying

⚙️ How It Works
A Python producer reads from a stock dataset (CSV), simulates live data, and streams it to a Kafka topic.

A Kafka broker, running on EC2, handles the message flow.

A Python consumer reads messages from Kafka and writes them to Amazon S3 in near real-time.

An AWS Glue Crawler scans the S3 bucket and updates the Glue Data Catalog.

Data is queried and analyzed using Amazon Athena with SQL.

📌 Key Highlights
Built a real-time data pipeline with event-driven architecture.

Integrated Kafka with AWS for scalable storage and analytics.

Enabled serverless querying of streaming data using Athena.

Demonstrated end-to-end flow from data ingestion → storage → querying.


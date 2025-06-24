# Stock-Market-Data-Pipeline-using-Kafka
This project simulates real-time stock market data streaming using Apache Kafka and processes it end-to-end with AWS services. A Python-based Kafka producer ingests data from a CSV dataset and streams it to a Kafka broker hosted on Amazon EC2. A Kafka consumer listens to this stream and writes the data to Amazon S3, which is then cataloged using AWS Glue and queried using Amazon Athena.

![Architecture](https://github.com/user-attachments/assets/8ccaf124-ccc8-46cc-9372-73ea1527e3cb)

## 🔧 Tech Stack
- **Apache Kafka** hosted on Amazon EC2  
- **Python** using:
  - `kafka-python` for Kafka integration  
  - `boto3` for AWS interactions  
  - `pandas` for data manipulation  
- **Amazon S3** for real-time data storage  
- **AWS Glue** for data cataloging  
- **Amazon Athena** for SQL-based querying over S3

---

## ⚙️ How It Works
- A **Python producer** reads data from a CSV-based stock dataset.
- It simulates live stock data and streams it to a **Kafka topic**.
- A **Kafka broker**, running on **EC2**, handles the message flow.
- A **Python consumer** reads messages from Kafka and writes them to **Amazon S3**.
- An **AWS Glue Crawler** scans the S3 bucket and updates the **Glue Data Catalog**.
- **Amazon Athena** is used to query and analyze the cataloged data using SQL.

---

## 📌 Key Highlights
- Built a **real-time data pipeline** using Kafka and AWS.
- Implemented **event-driven architecture** for data streaming.
- Integrated **Kafka with AWS S3, Glue, and Athena** for scalable analytics.
- Enabled **serverless SQL querying** over streaming data.
- Demonstrated end-to-end workflow from **data ingestion → storage → cataloging → querying**.


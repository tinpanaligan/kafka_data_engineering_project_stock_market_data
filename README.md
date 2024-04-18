# Real-time Stock Market Data Pipeline

---

## Overview

This project is aimed at creating a real-time data pipeline for stock market data using Python, Apache Kafka, AWS EC2, and AWS S3. The pipeline simulates real-time stock market data using historical CSV data, processes it using Python scripts, sends it to an Apache Kafka cluster hosted on AWS EC2, and finally consumes the data into AWS S3 for storage and further analysis.


![Kafka_Project_Architecture](https://github.com/tinpanaligan/kafka_data_engineering_project_stock_market_data/assets/116711183/e40f1380-60d1-4d16-bb49-07d1e8abec9d)



---

## Components

### 1. Stock Market CSV Data

- **Source**: Historical stock market data in CSV format.
- **Purpose**: To mimic real-time data by replaying historical data.

### 2. Python Scripts

- **Purpose**: Python scripts are used to read CSV data, transform it, and produce it to the Kafka cluster.

### 3. Apache Kafka

- **Purpose**: Apache Kafka is used as a distributed streaming platform to handle real-time data streams efficiently.
- **Deployment**: Kafka is hosted on an AWS EC2 instance for scalability and reliability.

### 4. AWS EC2 Instance

- **Purpose**: To host the Kafka cluster for real-time data processing.
- **Deployment**: Utilize AWS EC2 for its scalability and ease of deployment.

### 5. AWS S3

- **Purpose**: AWS S3 is used for storing the consumed stock market data for further analysis and long-term storage.
- **Consumption**: Consumed data from the Kafka cluster is stored in AWS S3 buckets.

---

## How to Run

1. **Set Up Apache Kafka on AWS EC2**:
   - Launch an EC2 instance on AWS.
   - Install Kafka on the EC2 instance following the Kafka documentation.

2. **Configure Kafka Cluster**:
   - Set up topics, partitions, and replication factors according to your requirements.

3. **Run Python Scripts**:
   - Modify the Python scripts to read CSV data, transform it, and produce it to the Kafka cluster.
   - Execute the Python scripts on a local machine or another EC2 instance to produce data to Kafka.

4. **Consume Data into AWS S3**:
   - Implement a Kafka consumer to consume data from the Kafka cluster.
   - Configure the consumer to store consumed data into AWS S3 buckets.

---

## Contributors

- Tin Panaligan

---

## Acknowledgments

Special thanks to Darshil Parmar for this project.

---

## Contact Information

For inquiries, please contact tinpanaligan.work@gmail.com.

---

## Appendix: Useful Resources

- [Apache Kafka Documentation](https://kafka.apache.org/documentation/)
- [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/index.html)
- [AWS S3 Documentation](https://docs.aws.amazon.com/s3/index.html)

---

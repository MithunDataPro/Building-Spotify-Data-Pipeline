# 🎵 Spotify Data Pipeline 🚀

## 📖 Overview
This project builds a **data pipeline for Spotify** using `AWS Glue`, `Apache Spark`, `Snowflake`, and `Power BI`. The goal is to extract **music streaming data** from the **Spotify API**, process it, and store it in **AWS S3** before loading it into **Snowflake** for analytics.

---

## 🏗️ Architecture Diagram
```plaintext
Spotify API → Amazon CloudWatch → Python (AWS Lambda) → AWS EMR → AWS S3 → AWS Glue (Apache Spark) → Trigger → S3 (Transformed Data) → Snowpipe → Snowflake → Power BI

```

## Workflow Explanation
1️⃣ Extract Data from Spotify API using AWS Lambda (Python script).
2️⃣ Schedule Extraction with Amazon CloudWatch (daily trigger).
3️⃣ Store Raw Data in Amazon S3 (JSON format).
4️⃣ Transform Data using Apache Spark on AWS Glue.
5️⃣ Trigger S3 Data Processing when new data arrives.
6️⃣ Load Transformed Data into Snowflake via Snowpipe.
7️⃣ Analyze Data using Power BI for visualization.



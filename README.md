# 🚀 AWS Glue ETL Pipeline for Cryptocurrency Data

![AWS Glue ETL Workflow](https://your-image-url.com)  <!-- Optional: Add an architecture diagram -->

## 📌 Project Overview  
This project is an **AWS Glue ETL pipeline** that:  
✅ **Extracts** cryptocurrency market data from the [CoinMarketCap API](https://coinmarketcap.com/api/)  
✅ **Transforms** the data using **AWS Glue (PySpark)**  
✅ **Loads** structured data into **Amazon S3 (Parquet) & DynamoDB**  
✅ **Automates** the ETL process using **AWS EventBridge**  

---

## 🔗 Architecture Overview  
1️⃣ **API Extraction → AWS Glue (Python & PySpark)**  
   - Requests live crypto data from CoinMarketCap API  
   - Flattens JSON & creates PySpark DataFrame  

2️⃣ **Data Transformation → AWS Glue (PySpark)**  
   - Cleans data, renames columns, handles missing values  

3️⃣ **Load to Storage**  
   - ✅ **S3 (Parquet format)** → For scalable storage  
   - ✅ **DynamoDB** → For real-time querying  

4️⃣ **Automation → AWS EventBridge**  
   - Runs AWS Glue job automatically (e.g., hourly)  

---

## 🛠 Technologies Used  
| Category          | Service / Tool |  
|-------------------|----------------|  
| **Programming**   | Python, PySpark (AWS Glue) |  
| **Data Extraction** | CoinMarketCap API (REST) |  
| **Data Processing** | AWS Glue (ETL, PySpark) |  
| **Storage**       | S3 (Parquet), DynamoDB |  
| **Automation**    | AWS EventBridge |  

---

## 📂 Project Structure  
```bash
aws-glue-crypto-etl/
│── glue_etl_script.py   # AWS Glue ETL script (PySpark)
│── requirements.txt     # Dependencies (if running locally)
│── README.md            # Documentation
│── architecture.png     # Optional: Workflow diagram

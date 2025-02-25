# aws-glue-pyspark-crypto-etl
Automated AWS Glue ETL pipeline that extracts live cryptocurrency market data from the CoinMarketCap API, transforms it using PySpark, and loads it into Amazon S3 (Parquet) &amp; DynamoDB for real-time querying. The pipeline is scheduled using AWS EventBridge.

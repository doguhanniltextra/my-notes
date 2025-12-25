
[[Athena Core]]

Athena charges you based on the amount of data scanned by each query. 
- Partitioning: This is the most important tool. By organizing your S3 data into a hierarchy.
	- _s3://my-bucket/logs/tenant_id=123/year=2025/month=12/day=24_ 
- Columnar Formats: Instead of CSV or JSON, store your data in Apache Parquet. This is a columnar format that allows Athena to read only the specific columns required for your query, significantly reducing the data scanned and improving performance.
- Since Athena supports reading compressed data, it scans fewer bytes, which directly reduces your bill.
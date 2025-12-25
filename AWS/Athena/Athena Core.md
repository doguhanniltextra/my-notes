
[[AWS]]

Amazon Athena is an interactive serverless query service that makes it easy to analyze data in Amazon S3 using standard SQL. Athena is the primary tool for _Log Analytics_ and _Data Lake Exploration_ allowing you to query massive amounts of IoT or HR data without the need to manage a database cluster.

Athena operates on a _Schema-on-read_ model, meaning the data remains in its raw format in S3, and you only define the structure when you want to query it.
- Serverless: There is nı infra to set up or manage. You don't _scale_ Athena; AWS handles the underleying compute power automatically based on the complexity of your query.
- Standard SQL: It uses **Trino** under the hood, supporting standard ANSI SQL. This allows you to perform complex joins, windows functions, and aggregations.

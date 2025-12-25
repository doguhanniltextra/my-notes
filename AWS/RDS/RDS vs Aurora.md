
[[RDS Core]] 

|**Feature**|**Standard RDS**|**Amazon Aurora**|
|---|---|---|
|**Replication**|Synchronous (Multi-AZ) / Asynchronous (Replicas)|Shared storage-based replication (6 copies across 3 AZs).|
|**Performance**|Standard SQL performance.|Up to 5x faster (MySQL) or 3x faster (PostgreSQL).|
|**Storage**|Fixed size with auto-scaling.|Auto-scaling up to 128 TiB.|
|**Failover Speed**|60–120 seconds.|Often less than 30 seconds.|
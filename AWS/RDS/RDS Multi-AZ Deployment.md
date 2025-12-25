
[[RDS Core]]

- Synchronous Replication: When you enable Multi-AZ, RDS automatically creates a Standby Instance in a different Availability Zone.
- Failover Mechanism: If the primary instance fails, RDS automatically flips the DNS CNAME to the standby instance. This typically happens in 60-120 seconds without manual intervention. 
- Primary vs Standby: The standby instance cannot serve read traffic, its sole purpose is failover.
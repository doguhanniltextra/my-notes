
[[RDS]]

The architecture of RDS is built on top of the standard AWS infra but abstracts the underlying EC2 instances and EBS volumes.
- DB Instance: The basic building block of RDS. It is an isolated database environment in the cloud. You choose the compute based on the instance class.
- Storage (EBS-backed): RDS uses _Amazon Elastic Block Store_ for storage. You can choose between:
	- General Purpose SSD (gp2/gp3): Balanced for most workloads.
	- Provisioned IOPS (io1): High-performance storage for I/O intensive applications.
- DB Engine: RDS supports multiple engines: MySQL, PostgreSQL, MariaDB, Oracle, SQL Server and Amazon Aurorra

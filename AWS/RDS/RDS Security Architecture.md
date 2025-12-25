
[[RDS]] 
- Network Isolation: RDS should always be placed in a Private Subnet within your VPC. It should not have a public IP.
- Security Groups: You must restrict access to the RDS port only to the Security Group of your _ECS Tasks._
- Encryption:
	- At Rest: Uses AWS KMS to encrypt the underlying storage, backups, and replicas.
	- In Transit: Uses SSL/TLS for all communication between your application and the database.
- IAM DB Authentication: You can authenticate to your database using IAM users or roles instead of fixed passwords, which aligns with your goal of managing _Task Roles_ effectively. 

[[AWS]]

It is a managed service that makes it easy for you to create and control the cryptographic keys used to protect your data.

- Core Architectural Concepts
KMS is built around the concept of KMS Keys. These keys never leave the KMS Hardware Security Modules unencrypted.
	- Customer Managed Keys: Keys you create, own, and manage. You have full control over their rotation policies and access permissions.
	- AWS Managed Keys: Keys created and managed by AWS services on your behalf. These are often named _aws/rds_ or _aws/s3_.
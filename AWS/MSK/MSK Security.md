
[[MSK Core]]

- VPC Integration: MSK is deployed within your Private subnets. It is not accessible from the public internet.
- Authentication: IAM is a secure method in MSK. Your ECS Task Role is granted permissions to produce or consume from specific topics.
	- SASL/SCRAM: Username and password stored in AWS Secrets Manager.
	- TLS: Uses certificates to verify identities, matching your existing mTLS strategy for agents.
	- Encryption: Data is encrypted using AWS KMS.
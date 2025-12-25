
[[CLI Configuration and Profiles]]

The CLI follows a predictable hierarchical structure:
	- `aws <service> <operation> <parameters> <options>`
- Service: The AWS service (ecs,rds,s3,secretsmanager)
- Operation: The action to perform (describe-tasks, list-buckets, get-secret-value)
- Parameters: Specific arguments like (--cluster, --secret-id)
- Global Options: Options like (--output json, --region us-east-1, --profile)


[[IAM Core]]

|**Type**|**Description**|**Best Practice**|
|---|---|---|
|**AWS Managed Policies**|Created and administered by AWS (e.g., `AmazonS3ReadOnlyAccess`).|Good for getting started, but often too broad for production.|
|**Customer Managed Policies**|Created by you. They provide standalone versions that can be attached to multiple users/roles.|**Recommended** for your **ECS Provider**roles to ensure granular control.|
|**Inline Policies**|Embedded directly into a single user, group, or role.|Avoid using these; they are harder to manage at scale across 400 companies.|
|**Resource-based Policies**|Attached directly to a resource (e.g., **S3 Bucket Policy** or **KMS Key Policy**).|Critical for cross-account access and services like **Secrets Manager**.|
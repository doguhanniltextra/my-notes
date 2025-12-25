
[[IAM Core]]

ARN is a standardized string used to uniquely identify any AWS resource across all of AWS. 

- ARN Syntax and Structure

Every ARN follows a specific hierarchical format. The structure varies slightly depending on the service, but the general format is:
	- arn:partition:service:region:account-id:resource-id

- Breakdown of Components
	- arn: This is the constant prefix that indicates the string is an Amazon Resource Name.
	- partition: The partition that the resource is in. For standard AWS regions, the partition is _aws_.
	- service: The service namespace that identifies the AWS product.
	- region: The region code where the resource resides. Some resources are global and leave this segment blank.
	- account-id: The 12-digiht AWS account member that owns the resource.
	- resource-id: The specific identifier for the resource. This can be name, a UUID, or a path-like structure.
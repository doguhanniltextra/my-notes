
[[Gateway]]

Private subnets host your sensitive workloads, such as RDS and ECS Tasks. These resources should never have a public IP.
- NAT Gateway (Network Address Translation)
	- Purpose: Allows resources in a private subnet to connect to the internet (e.g., to pull Docker images or establish a Cloudflare Tunnel) but prevents the internet from initiating a connection.
	- Placement: Must be placed in a Public Subnet.
- VPC Endpoints
	- Purpose: Allows you to connect your VPC to suppoerted AWS services (like Secrets Manager, S3, or ECR) privately without using an IGW or NAT Gateway.
	- Interface Endpoints: Uses an ENI with a private IP from your subnet.
	- Gateway Endpoints: A specific type for S3 and DynamoDB that you add as a target in your route table.
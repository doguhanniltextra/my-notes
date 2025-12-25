
[[Subnets]]

- Internet Gateway (IGW): Allows communication between your VPC and the internet. It is required for your Public Subnets.
- NAT Gateway: Located in the Public Subnet, It allows resources in the Private Subnet to reach the internet without allowing the internet to initiate a connection with them.
- VPC Endpoints: Allows you to connect your VPC to supported AWS services as if they were inside your VPC, avoiding the need for a NAT Gateway or IGW for that specific traffic.
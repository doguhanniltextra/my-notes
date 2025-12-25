[[Gateway]]

Public subnets are designed for resources that must be reachable from the internet or need to initiate direct communication with it.
- Internet Gateway (IGW): A horizontally scaled, redundant, and highly available VPC component that allows communication between your VPC and the internet.
	- Function: It performs Static Network Address Translation _NAT_ for your public resources.
	- Requirement: Your public route table must have a route with destination **0.0.0.0/0** and the IGW ID as the target.
- Egress-Only Internet Gateway: This is specifically for IPv6 traffic. It allows outbound communication from your VPC to the internet but prevents the internet from initiating a connection with your instances.
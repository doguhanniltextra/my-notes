
[[VPC Core]] 

- Public Subnets: These have a route to an Internet Gateway (IGW). This is where you place your _Network Load Balancer (NLB)_ and _Application Load Balancer (ALB)_ to receive incoming MQTT or HTTPS traffic.
- Private Subnets: These have no direct route to the internet. This is the _secure zone_ where you place your ECS Tasks and RDS databases.
- Multi-AZ Design: For high availability, you should always create subnets in at least two different Availability Zones (AZs).
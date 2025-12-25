
[[Route Tables Anatomy]]

- The _Local_ Route
	 Every route table contains a default _local_ route for the VPC's primary CIDR block. This route allows all subnets within the VPC to communicate with each other by default. You **cannot** delete or modify this route.
- Longest Prefix Match
	 If a packet matches multiple entries in a route table, AWS uses the most specific route.
- Main vs Custom Route Tables
	 - Main Route Table: The table that automatically comes with your VPC.
	 - Custom Route Table: Tables you create manually. It is a best practice to create custom tables for your _Public_ and _Private_ subnets to maintain strict isolation.

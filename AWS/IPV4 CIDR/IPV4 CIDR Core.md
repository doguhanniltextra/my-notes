
[[AWS]]

In the context of networking and AWS VPC design, CIDR is a method for allocating IP addresses and routing IP packets. It replaced the older _Classful_ networking system to allow for more flexible and efficient distribution of IP addresses.

When you create a VPC, the CIDR block defines the total range of private IP addresses that your VPC can utilize.

- Anatomy of a CIDR Block

A CIDR block is expressed in the format **[IP Address]/[Prefix Length]**.
	- IP Address: The starting point of the network (e.g., 10.0.0.0)
	- Prefix Length (The Suffix): Indicated by the _/_ followed by a number. This tells you how many bits are _masked_ for the network portion of the address.

- The Math Behind the Suffix

An IPv4 address consists of 32 bits. The suffix tells you how many of those bits are dedicated to the _Network ID_, while the remaining bits are for the Host ID.
	- Formula for Total IPs: 2 square(32 - suffix)
	- Example: (/16) = 
			32 - 16 = 16 bits for hosts.
			 2 square (16) = 65,536 addresses.

- AWS VPC Specifies

When setting your Primary CIDR block in AWS, there are strict rules and behaviors you must follow:
	- Allowed Sizes: AWS Allows VPC CIDR blocks between a _/16.  (maximum size, 65,536 IPs) and a _/28_ (minimum size, 16 IPs)
	- Reserved IPs: In every subnet you create within the VPC, AWS reserves 5 IP addresses for its own use:
		- x.x.x.0: Network addreses
		- x.x.x.1: VPC Router
		- x.x.x.2: Amazon Provided DNS
		- x.x.x.3: Reserved by AWS for future use
		- x.x.x.255: Network broadcast address (AWS doesn't support broadcast.)
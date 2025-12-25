
[[AWS]] 

Everything in a VPC starts with an IP range defined by a _CIDR_ block.
- Private Range: You typically choose a range from the RFC 1918 private address space.
- Primary CIDR: This provides up 65,536 private IP addresses.
- Architecture Tip: Ensure Your VPC CIDR does not overlap with your On-Premise network CIDR, otherwise, your Cloudflare Tunnel or VPN will face routing conflicts.
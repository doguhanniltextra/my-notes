
[[Route Tables Core]]

Every route consists of two primary components:
- Destination: The range of IP addresses where you want the traffic to go, defined in CIDR notation. (e.g. 10.0.0.0/16 for internal traffic or 0.0.0.0/0 for all internet traffic)
- Target: The gateway, network interface, or connection through which to send the destination traffic.
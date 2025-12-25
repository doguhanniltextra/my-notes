
[[AWS WAF]]


| **Feature**           | **L4 Firewall (Security Group)**   | **WAF (Layer 7)**                                   |
| --------------------- | ---------------------------------- | --------------------------------------------------- |
| **Inspection**        | IP, Port, Protocol (TCP/UDP).      | HTTP Headers, Cookies, JSON Body.                   |
| **Attack Prevention** | Prevents unauthorized port access. | Prevents SQLi, XSS, and Logic attacks.              |
| **MQTT Context**      | Blocks/Allows **Port 8883**.       | Does not inspect raw MQTT (unless over WebSockets). |
| **Placement**         | At the ENI/Instance level.         | At the Load Balancer or Edge level.                 |
[[Layer 7 - Load Balancer (Application Layer)]] 
Layer 4 load balancing operates at the intermediate **Transport Layer**, dealing with network protocols like TCP and UDP. It makes routing decisions based on network variables such as IP addresses and port numbers, without inspecting the actual content of the packets.
- Mechanism: It views the traffic as a stream of bytes. It does not "open" the packet to see what is inside.
- AWS Implementation: This is handled by the Network Load Balancer (NLB)
- Best Use Case: High-throughput, low latency applications like your MQTT IoT stream. Since it doesn't inspect data, it is extremely fast and can handle millions of requests per second with ultra-low latency.
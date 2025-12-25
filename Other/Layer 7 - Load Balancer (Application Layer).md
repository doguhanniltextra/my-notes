[[Layer 4 -  Load Balancer (Transport Layer)]] 
Layer 7 load balancing operates at the high-level Application Layer. It is "content-aware" meaning it can inspect the headers, cookies and the actual payload of the message. (eg., HTTP URLs, gRPC methods).
- Mechanism: It terminates the network connection and inspects the application-level data to make sophisticated routing decisions. For example, it can route /v1/hr to the HR-PROVIDER and /v1/isg to the ISG-PROVIDER based on the URL path.
- AWS Implementation: This is handled by the Application Load Balancer
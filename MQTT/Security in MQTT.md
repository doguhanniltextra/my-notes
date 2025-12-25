[[MQTT Technical Concepts]]

Since you are bypassing the Cloudflare Tunnel for MQTT and going directly to an AWS NLB, security must be handled at the protocol level:
	- MQTTS (_PORT 8883_): Always use TLS encryption for data in transit.
	- mTLS (Mutual TLS): Both the client and the broker must present certificates to verify their identities.

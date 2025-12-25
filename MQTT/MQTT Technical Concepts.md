- Topics and Filter
Topics are hierarchical strings used by the broker to filter messages for each connected client.
	- Structure: You can assign your Custom ID hierarchy here.

- Quality of Service (QoS) Levels
	- QoS 0 (At most once): The message is sent once; no acknowledgement is required. Best for high-frequency, non-critical data.
	- QoS 1 (At least once): Ensures the message reaches the broker at least once but may result in duplicates. (Recommended for IoT data.)
	- QoS 2 (Exactly once): The safest but slowest level, involving a four-step handshake to ensure no duplicates.
	
- Last Will and Testament (LWT)
	- If a client disconnects ungracefully, the broker automatically publishes a pre-defined "Last Will" message to a specific topic. This is critical for real-time monitoring of yor on-premise infra health.
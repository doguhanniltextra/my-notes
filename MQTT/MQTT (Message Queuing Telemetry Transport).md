MQTT is a lightweight, publish-subscribe network protocol that transports messages between devices. It is the industry standard for IoT due to its effeciency in high-latency, low-bandwith, or unreliable networks.

- MQTT Client: In your architecture, Agent 3 acts as the client. It can either publish data (telemetry) or subscribe to commands (_reboot_ signal from the Cloud)
- MQTT Broker: The central hub that receives all messages, filters them and decides who is interested in them. 

### Note:
- Publisher and subscriber do not need to know each other's IP addresses.
- They do not need to be connected at the same time.
- Operations on both ends do not halt during waiting for messages.

[[MQTT Technical Concepts]]
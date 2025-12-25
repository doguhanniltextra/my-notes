[[MQTT (Message Queuing Telemetry Transport)]] 

|**Feature**|**MQTT (for IoT)**|**gRPC (for CRUD/Auth)**|
|---|---|---|
|**Pattern**|Pub/Sub|Request/Response|
|**Network**|Excellent for unstable links|Requires stable connection|
|**Overhead**|Minimal (2-byte header)|Higher (HTTP/2 framing)|
|**Use Case**|Continuous telemetry streams|Database records / UI Actions|

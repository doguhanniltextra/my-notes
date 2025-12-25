
[[Elastic Container Service IAM Roles]] 

Modern ECS deployments almost exclusively use the _awsvpc_ network mode.

- ENI (Elastic Network Interface): Each task get its own dedicated ENI and private IP address from your VPC.
- Security Groups: You can apply fine-grained firewall rules at the task level. For instance, you can allow MQTT (Port 8883) only from your on-premise IP while blocking all other traffic.
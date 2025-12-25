
[[Elastic Container Service (ECS)]] 

- Rolling Updates: When you push a new image to ECR, ECS spins up new tasks before shutting down the old ones, ensuring zero downtime for your customers.
- Service Auto Scaling: You can scale the number of tasks based on CPU utilization or custom metrics like the number of incoming MQTT messages from your NLB.

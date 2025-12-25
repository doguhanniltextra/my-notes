[[AWS]] 
ECS organizes resources in a structured hierarchy that separates administrative grouping from actual compute execution:
- Cluster: A logical grouping of services or tasks. It acts as an isolation boundary for your _Cloud Region_.
- Service: Responsible for maintaining the _Desired State_. If a task fails, the service automatically restarts it to maintain the specified count of instances. This is where the services reside.
- Task Definition: A blueprint (in JSON) that defines how a container should run. It specifies the Docker image, CPU/Memory limits, environment variables, and storage volumes.
- Task: The smallest deployable unit in ECS. It is a running instance of a _Task Definition_.




[[AWS]]

Amazon MSK is a fully managed service that makes it easy to build and run applications that use Apache Kafka to process streaming data. It handles the operational overhead of managing kafka clusters, including setup, configuration, and maintenance.
- Core Architectural Components: 
	- Brokers: These are the EC2 instances that host the kafka pratitions and handle read/write requests. In a production environment, you should use at least 3 brokers across 3 AZs.
	- Zookeper Nodes: MSK manages Apache ZooKeeper nodes to coordinate the cluster and manage the state of brokers and topics.
	- Storage: Each broker is backed by Amazon EBS volumes. You can scale storage independently of compute.

|**Concept**|**Description**|**Application in Your Project**|
|---|---|---|
|**Topics**|Categories used to organize messages.|`telemetry.isg.raw` or `events.hr.updates`.|
|**Partitions**|Subdivisions of a topic for parallelism.|Allows multiple **ECS Task** instances to read from the same topic simultaneously.|
|**Consumer Groups**|A group of consumers working together to consume data.|Ensures that each IoT message is processed exactly once by your providers.|
|**Replication Factor**|The number of copies of data maintained.|Typically set to 3 to ensure data is not lost if a broker fails.|

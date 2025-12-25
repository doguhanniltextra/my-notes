
[[AWS]]

## The Four Pillars of CloudWatch

- CloudWatch Logs
CloudWatch Logs allows you to centralize the logs from all your systems, including your on-premise agents and cloud providers.

- CloudWatch Metrics
	-  Standard Metrics: Automatically provided by AWS services.
	- Custom Metrics: You can publish your own data poits, such as _Number of MQTT messages processed per factory_ or _Zstd compression ratio_.
	- Dimensions: Key-Value pairs that allow you to filter and aggregate metrics for specific tenants.
- CloudWatch Alarms
	- Static Threshold: Triggers if a metric exceeds a set value
	- Anomaly Detection: Uses ML to analyze historical data and detect unusual spikes in your IoT data flow.
	- Actions: Can trigger Auto Scaling for your ECS services, send notifications via SNS, or execute a Lambda function for automated remediation.
- CloudWatch Dashboards
	- Unified View: You can combine cloud metrics and on-premise status into a single glass pane.
	- If you expand to multiple AWS regions, you can aggregate data into one dashboard.


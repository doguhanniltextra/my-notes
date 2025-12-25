
[[AWS]]

CloudTrail captures a history of AWS API calls for your account. These include actions taken via:
- AWS Management Console
- AWS SDKs
- CLI
- Other AWS Services

### Key Components of a CloudTrail Event

When an event is recorded, CloudTrail provides detailed metadata:
- Identity: Which IAM user or role made the request?
- Timestamp: When did the action occur?
- Source IP: From which IP address was the request initiated?
- Parameters: What were the request parameters?
- Response: Was the request sucessful or denied?
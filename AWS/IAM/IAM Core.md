
 [[AWS]]

In AWS, an IAM Policy is a JSON document that defines permissions. It specifies what actions are allowed or denied on which resources, and under what conditions. 

- Anatomy of a JSON Policy Statement

A policy consists of one or more statements. Each statement includes the following elements.
	- Version: The policy language version
	- Statement ID (Sid): An optional identifier for the statement
	- Effect: Either _Allow_ or _Deny_
	- Action: The specific API calls being allowed or denied
	- Resource: The specific AWS resource the actions apply to, identified by an _[[ARN]]_
	- Condition: (Optional) Circumstances under which the policy is in effect
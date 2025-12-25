
[[CLI Core]]

Before running commands, you must provide credentials.
- aws configure: The primary command to set up your Access Key ID, Secret Access Key, Default Region, and Output Format.
- Named Profiles: You can manage multiple AWS accounts or environments by using profiles:
	- `aws configure --profile hr-account.`
- Precedence: Credentials can be provided via environment variables, the configuration file, or an IAM instance/task role.
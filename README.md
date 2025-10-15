# AWS_Attack_Detection_soclabs
This repo would contain all 17 AWS attack related scenarios present there at https://www.soc-labs.top/en/detection

## Scenarios:

|  n | Scenario | Objective | Detection Query (Sigma) | 
| -- | -------- | -------- | ---- |
| 1. | AWS Delete DNS query logs | Detect the deletion of Route 53 DNS resolver query logs in AWS environments | link |
| 2. | AWS EC2 Windows Instance Password Data Retrieval | Write detection rules to identify password data retrieval activities targeting Windows EC2 instances in an AWS environment, with a focus on `ec2:GetPasswordData` API call events. | link |
| 3. | EC2 Credential Exfiltration – EC2 Account Credentials Used by Another AWS Account | Identify all API operations initiated with EC2 instance credentials where the credential’s originating account does not match the account where the API call occurs. | link |
| 4. | Retrieving a High Number of AWS Secrets Manager Secrets | Write detection rules to identify abnormal Secrets Manager secret retrieval activities. Focus on suspicious behavior patterns related to Secrets Manager. | link |
| 5. | Retrieve And Decrypt SSM Parameters | Write detection rules to identify suspicious bulk decryption of `SecureString` parameters. When a request sets the `withDecryption` parameter to `true`, it indicates an attempt to retrieve parameter plaintext. Focus on operations that decrypt multiple SecureString parameters within a short time window to identify potential sensitive information leakage risks. | link |
| 6. | AWS Deletes a trail | Write detection rules based on logs to identify API calls that delete a Trail. | link |
| 7. | Disabling Management Event Logging via Event Selector | Write a detection rule to identify calls to the `PutEventSelectors` API. | link |
| 8. | CloudTrail Logs Impairment Through S3 Lifecycle Rule | Write a rule to identify log entries where the S3 bucket lifecycle policy is set to 1 day. | link |


[[Types of IAM]]


`{`
    `"Version": "2012-10-17",`
    `"Statement": [`
        `{`
            `"Effect": "Allow",`
            `"Action": "rds-db:connect",`
            `"Resource": "arn:aws:rds-db:us-east-1:123456789012:dbuser:cluster-ABC/db_user_name"`
        `},`
        `{`
            `"Effect": "Allow",`
            `"Action": [`
                `"secretsmanager:GetSecretValue",`
                `"kms:Decrypt"`
            `],`
            `"Resource": [`
                `"arn:aws:secretsmanager:us-east-1:123456789012:secret:my_db_secret",`
                `"arn:aws:kms:us-east-1:123456789012:key/my_kms_key_id"`
            `]`
        `}`
    `]`
`}`
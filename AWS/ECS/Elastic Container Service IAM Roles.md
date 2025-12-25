
[[Elastic Container Service - Deployment]]

| **Role Type**           | **Purpose**                             | **Example for Your Project**                                       |
| ----------------------- | --------------------------------------- | ------------------------------------------------------------------ |
| **Task Execution Role** | Used by the ECS Agent itself.           | Pulling images from **ECR**, sending logs to **CloudWatch**.       |
| **Task Role**           | Used by the code inside your container. | Your **HR-PROVIDER** accessing an **S3 Bucket** to retrieve a PDF. |

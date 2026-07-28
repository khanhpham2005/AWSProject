---
title: "Week 5 Worklog"
date: 2026-06-29
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 objectives

* Deploy the back-end to AWS Lambda in a fully serverless architecture.
* Attach a dedicated IAM Role and test the Lambda function independently.

### Tasks during the week (29/06 - 03/07/2026)

| Day | Task | Start | End | Reference |
| --- | --- | --- | --- | --- |
| Mon | Write a custom Lambda handler routing API Gateway HTTP events by method/path, then package it as a ZIP file for Python runtime deployment. | 29/06/2026 | 29/06/2026 | [Serverless lab](https://000078.awsstudygroup.com) |
| Tue | Mitigate cold start impact by tuning memory (512 MB), timeout (15s), and sourcing configs from environment variables. | 30/06/2026 | 30/06/2026 |  |
| Wed | Create an Execution Role for Lambda combining `AWSLambdaBasicExecutionRole` and a least-privilege inline policy scoped to the S3 bucket. | 01/07/2026 | 01/07/2026 | [IAM Role](https://000048.awsstudygroup.com) |
| Thu | Manage environment variables (bucket name, region, DynamoDB table name) to ensure unified codebase execution across local and cloud environments. | 02/07/2026 | 02/07/2026 |  |
| Fri | Execute standalone Lambda tests using direct `invoke` with mock payloads and verify output via CloudWatch Logs. | 03/07/2026 | 03/07/2026 |  |

### Results achieved

1. Successfully ran back-end logic fully serverless on Lambda with optimized cold start and memory configuration.
2. Configured a dedicated least-privilege IAM Execution Role for Lambda.
3. Completed independent Lambda function testing and verified CloudWatch logs prior to API Gateway integration.

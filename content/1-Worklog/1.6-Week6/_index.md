---
title: "Week 6 Worklog"
date: 2026-07-06
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 objectives

* Expose public endpoints for the frontend via API Gateway.
* Complete the end-to-end integration workflow on AWS.

### Tasks during the week (06/07 - 10/07/2026)

| Day | Task | Start | End | Reference |
| --- | --- | --- | --- | --- |
| Mon | Create an HTTP API Gateway with Lambda proxy integration and define routes (`POST /files`, `GET /files`, `GET /files/{id}`). | 06/07/2026 | 06/07/2026 | [API Gateway lab](https://000079.awsstudygroup.com) |
| Tue | Configure CORS settings on API Gateway and grant invocation permissions to trigger Lambda. | 07/07/2026 | 07/07/2026 |  |
| Wed | Update the frontend configuration to point calls to the API Gateway Invoke URL instead of local API. | 08/07/2026 | 08/07/2026 |  |
| Thu | Test APIs using Postman and frontend, resolve CORS preflight issues and IAM permission errors. | 09/07/2026 | 09/07/2026 | Postman |
| Fri | Review and finalize the end-to-end processing pipeline from Frontend to S3 on AWS. | 10/07/2026 | 10/07/2026 |  |

### Results achieved

1. API Gateway operational with public endpoints and properly configured CORS for frontend integration.
2. Successfully switched frontend requests from local backend to API Gateway.
3. Resolved integration issues and completed the full serverless end-to-end workflow on the cloud.

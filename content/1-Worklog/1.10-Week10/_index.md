---
title: "Week 10 Worklog"
date: 2026-08-03
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 objectives

* Implement file content search and host the frontend on S3 + CloudFront.
* Set up CloudWatch monitoring and optimize operational costs.

### Tasks during the week (03/08 - 07/08/2026)

| Day | Task | Start | End | Reference |
| --- | --- | --- | --- | --- |
| Mon | Query image labels (Rekognition) and extracted text (Textract) in DynamoDB matching user search keywords. | 03/08/2026 | 03/08/2026 |  |
| Tue | Develop the `/ask` endpoint supporting Q&A across the entire document library with detailed file source citations. | 04/08/2026 | 04/08/2026 |  |
| Wed | Host static frontend on S3 integrated with CloudFront (HTTPS, Origin Access Control) to secure the private bucket. | 05/08/2026 | 05/08/2026 | [CloudFront](https://cloudjourney.awsstudygroup.com/1-explore/) |
| Thu | Configure Lambda log forwarding to CloudWatch and set up CloudWatch Alarms for function error metrics. | 06/08/2026 | 06/08/2026 |  |
| Fri | Optimize costs (S3 Lifecycle Rules, CloudFront Caching TTL) and audit all IAM policies for least-privilege compliance. | 07/08/2026 | 07/08/2026 |  |

### Results achieved

1. Completed file content search and the library-wide `/ask` endpoint with specific file source citations.
2. Deployed frontend securely via CloudFront + S3 using HTTPS and Origin Access Control.
3. Integrated CloudWatch monitoring, optimized storage/data transfer costs, and enforced strict IAM permissions.

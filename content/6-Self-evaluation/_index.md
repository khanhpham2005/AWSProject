---
title: "Self-Assessment"
date: 2026-06-01
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

Internship at **Amazon Web Services Vietnam Company Limited** (First Cloud AI Journey program) from **June 01, 2026** to **August 15, 2026**.

Primary project: **InsightShare** – a serverless web app for uploading and sharing images/documents on AWS. Built using Python (`boto3`) alongside S3, Lambda, API Gateway, DynamoDB, CloudFront, IAM, and CloudWatch; with bilingual documentation.

Self-evaluation across 8 criteria:

| No. | Criteria | Good | Fair | Comments |
| --- | --- | --- | --- | --- |
| 1 | **Technical Skills** | x | | Successfully applied core AWS services to an end-to-end project. |
| 2 | **Learning Agility** | x | | Proactively self-taught new technologies (Lambda, presigned URLs, CloudFront) via docs & labs. |
| 3 | **Proactiveness** | x | | Took initiative in system design and service selection research. |
| 4 | **Discipline** | | x | Maintained fixed office attendance and submitted weekly worklogs on time. |
| 5 | **Communication** | x | | Reported progress clearly and delivered comprehensive bilingual documentation. |
| 6 | **Team Collaboration** | | x | Integrated well, actively consulted mentors, and supported teammates. |
| 7 | **Problem-Solving** | x | | Utilized CloudWatch logs to troubleshoot integration issues (CORS, IAM, cold start, S3 307, DynamoDB `Decimal`). |
| 8 | **Project Contribution** | x | | Built InsightShare end-to-end and added extra features (file deletion, expiring links, upload limits). |

### Lesson Learned

* S3 presigned URLs in Singapore require explicit regional endpoints and Signature V4 to prevent HTTP 307 errors.
* Lambda caches execution environment credentials; functions must be redeployed/updated to apply new IAM policies.
* `text` is a DynamoDB reserved keyword, requiring `ExpressionAttributeNames` for update expressions.
* DynamoDB returns numbers as `Decimal` objects, necessitating a custom JSON encoder for `json.dumps` serialization.
* AI integrations (Textract, Bedrock) must fail soft to keep the core pipeline operational during service degradation.
* CloudWatch logs serve as the primary diagnostic tool for serverless applications.

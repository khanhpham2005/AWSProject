---
title: "Week 4 Worklog"
date: 2026-06-22
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 objectives

* Integrate Amazon S3 as primary storage using presigned URLs.
* Configure CORS and implement least-privilege IAM policies for storage.

### Tasks during the week (22/06 - 26/06/2026)

| Day | Task | Start | End | Reference |
| --- | --- | --- | --- | --- |
| Mon | Create a private S3 bucket in ap-southeast-1, enable Block Public Access, and default SSE-S3 encryption. | 22/06/2026 | 22/06/2026 | [Amazon S3](https://000057.awsstudygroup.com) |
| Tue | Implement presigned URL generation (upload/download) using `boto3` with a 15-minute expiration and test via `curl`. | 23/06/2026 | 23/06/2026 |  |
| Wed | Configure S3 bucket CORS rules to allow direct browser uploads via presigned URLs. | 24/06/2026 | 24/06/2026 |  |
| Thu | Integrate S3 Storage into the interface layer built in Week 3 without modifying business logic. | 25/06/2026 | 25/06/2026 |  |
| Fri | Author a least-privilege IAM policy scoped strictly to S3 actions and test error scenarios (expired URLs, invalid keys). | 26/06/2026 | 26/06/2026 |  |

### Results achieved

1. Stored files securely in a private S3 bucket accessed via presigned URLs without public exposure.
2. Successfully migrated storage to S3 with zero impact on core business logic thanks to the decoupled interface.
3. Applied least-privilege access early and validated edge cases and error handling.

---
title: "Week 11 Worklog"
date: 2026-08-10
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 objectives

* Perform end-to-end testing, optimize performance, and finalize the system.
* Automate deployment workflows and clean up all AWS resources.

### Tasks during the week (10/08 - 14/08/2026)

| Day | Task | Start | End | Reference |
| --- | --- | --- | --- | --- |
| Mon | Write a deployment script to automate packaging (ZIP) and code updates via `aws lambda update-function-code`. | 10/08/2026 | 10/08/2026 |  |
| Tue | Conduct end-to-end and edge-case testing (large files, expired presigned URLs, permission errors, concurrent uploads). | 11/08/2026 | 11/08/2026 | Postman |
| Wed | Measure AI processing latency and search speeds via CloudWatch, fine-tuning Lambda memory allocations accordingly. | 12/08/2026 | 12/08/2026 |  |
| Thu | Develop a resource cleanup script (`cleanup-aws.ps1`) and document AWS Step Functions usage for future multi-step AI orchestration. | 13/08/2026 | 13/08/2026 | [Modernize](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| Fri | Record the product demo video and finalize the bilingual project report. | 14/08/2026 | 14/08/2026 |  |

### Results achieved

1. Fully scripted deployment and cleanup processes into single commands (ZIP + `update-function-code` and `cleanup-aws.ps1`).
2. Completed end-to-end testing, gracefully handled error scenarios, and reduced Lambda execution latency using CloudWatch metrics.
3. Delivered a complete project package including a demo video, bilingual report, and architecture notes on scaling AI pipelines via Step Functions.

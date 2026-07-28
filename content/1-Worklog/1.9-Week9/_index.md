---
title: "Week 9 Worklog"
date: 2026-07-27
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 objectives

* Integrate AI services to analyze and understand file content on a per-user basis.
* Utilize AWS managed AI services instead of self-training models.

### Tasks during the week (27/07 - 31/07/2026)

| Day | Task | Start | End | Reference |
| --- | --- | --- | --- | --- |
| Mon | Study FCAJ's AI services workshop, determining integration points for Rekognition and Textract within the upload pipeline. | 27/07/2026 | 27/07/2026 | [AI services](https://000056.awsstudygroup.com) |
| Tue | Integrate Amazon Rekognition (`detect_labels`) to automatically tag uploaded image files. | 28/07/2026 | 28/07/2026 |  |
| Wed | Utilize Amazon Textract (`detect_document_text`) to extract text from PDFs/images, and directly read `.txt` files from S3. | 29/07/2026 | 29/07/2026 |  |
| Thu | Develop the `POST /files/{id}/ask` endpoint connecting to Claude on Amazon Bedrock (`invoke_model`) for document Q&A and summarization. | 30/07/2026 | 30/07/2026 | [Bedrock](https://docs.aws.amazon.com/bedrock/) |
| Fri | Extend IAM Role permissions (Rekognition/Textract/Bedrock), store labels and text in DynamoDB by owner, and test the full pipeline. | 31/07/2026 | 31/07/2026 |  |

### Results achieved

1. Automated image tagging (Rekognition) and text extraction (Textract/S3), storing analytical data per user.
2. Completed document Q&A and summarization features via Bedrock (Claude) supporting multi-language responses with a fail-soft mechanism to prevent flow disruptions.
3. Stored AI metadata in DynamoDB as a foundation for search functionality, enforcing least-privilege IAM policies.

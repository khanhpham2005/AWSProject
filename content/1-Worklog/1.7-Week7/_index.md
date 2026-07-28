---
title: "Week 7 Worklog"
date: 2026-07-13
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 objectives

* Integrate DynamoDB to manage file metadata.
* Serve file downloads/views via presigned URLs and ensure data consistency.

### Tasks during the week (13/07 - 17/07/2026)

| Day | Task | Start | End | Reference |
| --- | --- | --- | --- | --- |
| Mon | Create a DynamoDB table (On-Demand mode, Partition Key: fileId) tailored for lookup and file listing needs. | 13/07/2026 | 13/07/2026 | [DynamoDB lab](https://000078.awsstudygroup.com) |
| Tue | Update Lambda to write metadata (`put_item`) and retrieve file information (`query`/`get_item`). | 14/07/2026 | 14/07/2026 |  |
| Wed | Synchronize S3 and DynamoDB data: record metadata only after successful S3 file upload. | 15/07/2026 | 15/07/2026 |  |
| Thu | Add restricted `dynamodb:PutItem`, `GetItem`, and `Query` permissions for the table to the Lambda IAM Role. | 16/07/2026 | 16/07/2026 |  |
| Fri | Configure the `get_file` API to return a short-lived presigned GET URL for viewing/downloading files and test the full flow. | 17/07/2026 | 17/07/2026 |  |

### Results achieved

1. Stored and queried metadata on DynamoDB independently from file contents in S3.
2. Ensured data consistency between S3 and DynamoDB.
3. Completed file viewing/downloading via presigned URLs and successfully tested the entire system.

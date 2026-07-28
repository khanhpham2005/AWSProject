---
title: "Worklog Tuần 2"
date: 2026-06-08
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2

* Thiết kế kiến trúc InsightShare và hoàn thiện Proposal.
* Thiết lập tài khoản AWS an toàn và cấu hình môi trường ban đầu.
* Nghiên cứu presigned URL và cơ chế hoạt động của các dịch vụ AWS AI.

### Các công việc trong tuần (08/06 - 12/06/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Nghiên cứu AWS IAM: user, group, role, phân biệt identity/resource policy và nguyên tắc least-privilege. | 08/06/2026 | 08/06/2026 | [AWS IAM](https://000002.awsstudygroup.com) |
| 3 | Vẽ sơ đồ kiến trúc serverless InsightShare (CloudFront, S3, API Gateway, Lambda, DynamoDB, Rekognition, Textract, Bedrock). | 09/06/2026 | 09/06/2026 | [draw.io](https://draw.io/) |
| 4 | Viết Proposal: phân tích bài toán, giải pháp và danh sách 10 dịch vụ AWS chọn dùng tại region `ap-southeast-1`. | 10/06/2026 | 10/06/2026 |  |
| 5 | Khởi tạo tài khoản AWS: bật MFA cho Root, tạo IAM User làm việc, cấu hình AWS CLI và đặt AWS Budget cảnh báo chi phí. | 11/06/2026 | 11/06/2026 |  |
| 6 | Thiết kế schema DynamoDB cho metadata file; nghiên cứu luồng presigned URL và cách gọi API các dịch vụ AI. | 12/06/2026 | 12/06/2026 | [AI services](https://000056.awsstudygroup.com) |

### Kết quả đạt được

1. Hoàn thành sơ đồ kiến trúc serverless và đề xuất Proposal chi tiết cho hệ thống InsightShare.
2. Thiết lập môi trường AWS an toàn (MFA, IAM User, AWS CLI, Budgets).
3. Nắm vững cơ chế presigned URL và cách thức tích hợp các API AI managed của AWS.

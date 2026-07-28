---
title: "Worklog Tuần 5"
date: 2026-06-29
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5

* Triển khai back-end lên AWS Lambda theo mô hình serverless.
* Thiết lập IAM Role và kiểm thử hàm Lambda độc lập.

### Các công việc trong tuần (29/06 - 03/07/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Viết Lambda handler điều hướng request theo method/path và đóng gói file zip deploy lên runtime Python. | 29/06/2026 | 29/06/2026 | [Serverless lab](https://000078.awsstudygroup.com) |
| 3 | Tối ưu thời gian cold start bằng cách điều chỉnh bộ nhớ (512 MB), timeout (15s) và dùng biến môi trường. | 30/06/2026 | 30/06/2026 |  |
| 4 | Tạo Execution Role cho Lambda gồm `AWSLambdaBasicExecutionRole` và inline policy giới hạn quyền truy cập S3 bucket. | 01/07/2026 | 01/07/2026 | [IAM Role](https://000048.awsstudygroup.com) |
| 5 | Quản lý cấu hình linh hoạt qua biến môi trường (bucket name, region, DynamoDB table) để code chạy tương thích cả local và cloud. | 02/07/2026 | 02/07/2026 |  |
| 6 | Thực thi test trực tiếp Lambda qua lệnh `invoke` với payload mẫu và kiểm tra log chi tiết trên CloudWatch. | 03/07/2026 | 03/07/2026 |  |

### Kết quả đạt được

1. Triển khai thành công back-end serverless trên Lambda, tối ưu tốt tài nguyên và thời gian cold start.
2. Thiết lập IAM Execution Role riêng chuẩn least-privilege cho Lambda.
3. Hoàn tất kiểm thử độc lập hàm Lambda và theo dõi log trên CloudWatch trước khi nối API Gateway.

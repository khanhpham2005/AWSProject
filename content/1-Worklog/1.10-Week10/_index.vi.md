---
title: "Worklog Tuần 10"
date: 2026-08-03
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10

* Triển khai tìm kiếm nội dung file và host frontend trên S3 + CloudFront.
* Thiết lập giám sát CloudWatch và tối ưu chi phí vận hành.

### Các công việc trong tuần (03/08 - 07/08/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Phân tích và truy vấn dữ liệu nhãn (Rekognition) và text (Textract) trong DynamoDB theo từ khóa của từng user. | 03/08/2026 | 03/08/2026 |  |
| 3 | Phát triển endpoint `/ask` hỗ trợ hỏi đáp trên toàn bộ thư viện tài liệu kèm trích dẫn nguồn file chi tiết. | 04/08/2026 | 04/08/2026 |  |
| 4 | Host static frontend trên S3 kết hợp CloudFront (HTTPS, Origin Access Control) để bảo mật bucket private. | 05/08/2026 | 05/08/2026 | [CloudFront](https://cloudjourney.awsstudygroup.com/1-explore/) |
| 5 | Cấu hình log Lambda chuyển tiếp CloudWatch và thiết lập CloudWatch Alarm cảnh báo khi phát sinh lỗi. | 06/08/2026 | 06/08/2026 |  |
| 6 | Tối ưu chi phí (S3 Lifecycle Rules, CloudFront Caching TTL) và rà soát toàn bộ IAM policies chuẩn least-privilege. | 07/08/2026 | 07/08/2026 |  |

### Kết quả đạt được

1. Hoàn thiện tìm kiếm nội dung file và endpoint `/ask` tổng hợp thông tin kèm trích dẫn nguồn cụ thể.
2. Triển khai frontend an toàn qua CloudFront + S3 với HTTPS và Origin Access Control.
3. Tích hợp giám sát CloudWatch, tối ưu chi phí lưu trữ/truyền tải và siết chặt phân quyền IAM.

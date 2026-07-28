---
title: "Worklog Tuần 7"
date: 2026-07-13
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7

* Tích hợp DynamoDB để quản lý metadata file.
* Phục vụ tải/xem file qua presigned URL và đảm bảo tính nhất quán dữ liệu.

### Các công việc trong tuần (13/07 - 17/07/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Tạo bảng DynamoDB (chế độ On-Demand, Partition Key: fileId) phù hợp với nhu cầu tra cứu và liệt kê file. | 13/07/2026 | 13/07/2026 | [DynamoDB lab](https://000078.awsstudygroup.com) |
| 3 | Cập nhật Lambda ghi metadata (`put_item`) và truy vấn thông tin file (`query`/`get_item`). | 14/07/2026 | 14/07/2026 |  |
| 4 | Đồng bộ dữ liệu S3 và DynamoDB: chỉ lưu metadata sau khi file đã tải lên S3 thành công. | 15/07/2026 | 15/07/2026 |  |
| 5 | Bổ sung các quyền `dynamodb:PutItem`, `GetItem`, `Query` giới hạn cho bảng vào IAM Role của Lambda. | 16/07/2026 | 16/07/2026 |  |
| 6 | Cấu hình API `get_file` trả về presigned GET URL ngắn hạn để xem/tải file và kiểm thử toàn bộ luồng. | 17/07/2026 | 17/07/2026 |  |

### Kết quả đạt được

1. Lưu trữ và truy vấn metadata trên DynamoDB độc lập với nội dung file ở S3.
2. Đảm bảo tính nhất quán dữ liệu giữa S3 và DynamoDB.
3. Hoàn thiện tính năng xem/tải file qua presigned URL và kiểm thử thành công toàn bộ hệ thống.

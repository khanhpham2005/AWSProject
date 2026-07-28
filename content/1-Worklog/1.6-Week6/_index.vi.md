---
title: "Worklog Tuần 6"
date: 2026-07-06
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6

* Mở endpoint public cho frontend qua API Gateway.
* Hoàn thiện luồng tích hợp end-to-end trên AWS.

### Các công việc trong tuần (06/07 - 10/07/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Tạo HTTP API Gateway (Lambda proxy) và định nghĩa các route (`POST /files`, `GET /files`, `GET /files/{id}`). | 06/07/2026 | 06/07/2026 | [API Gateway lab](https://000079.awsstudygroup.com) |
| 3 | Cấu hình CORS trên API Gateway và cấp quyền cho phép Gateway kích hoạt Lambda. | 07/07/2026 | 07/07/2026 |  |
| 4 | Cập nhật frontend chuyển sang gọi Invoke URL của API Gateway thay cho local API. | 08/07/2026 | 08/07/2026 |  |
| 5 | Kiểm thử API qua Postman/Frontend, khắc phục lỗi CORS preflight và phân quyền IAM. | 09/07/2026 | 09/07/2026 | Postman |
| 6 | Rà soát và tối ưu toàn bộ luồng xử lý end-to-end từ Frontend đến S3 trên AWS. | 10/07/2026 | 10/07/2026 |  |

### Kết quả đạt được

1. API Gateway chạy ổn định, hỗ trợ CORS đúng cho frontend.
2. Frontend chuyển đổi thành công sang gọi API trên cloud.
3. Khắc phục triệt để lỗi tích hợp, hoàn tất luồng end-to-end serverless.

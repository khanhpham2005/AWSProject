---
title: "Worklog Tuần 11"
date: 2026-08-10
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11

* Kiểm thử end-to-end, tối ưu hiệu năng và hoàn thiện hệ thống.
* Tự động hóa quy trình triển khai và dọn dẹp toàn bộ tài nguyên.

### Các công việc trong tuần (10/08 - 14/08/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Viết script tự động hóa deployment (đóng gói ZIP và gọi `aws lambda update-function-code`). | 10/08/2026 | 10/08/2026 |  |
| 3 | Thực hiện kiểm thử end-to-end và test các kịch bản lỗi (file lớn, presigned URL hết hạn, sai phân quyền, tải đồng thời). | 11/08/2026 | 11/08/2026 | Postman |
| 4 | Đo đạc thời gian xử lý AI/tìm kiếm qua CloudWatch và tinh chỉnh dung lượng bộ nhớ (Memory) của Lambda. | 12/08/2026 | 12/08/2026 |  |
| 5 | Phát triển script dọn dẹp tài nguyên (`cleanup-aws.ps1`) và nghiên cứu ứng dụng Step Functions cho pipeline AI. | 13/08/2026 | 13/08/2026 | [Modernize](https://cloudjourney.awsstudygroup.com/4-modernize/) |
| 6 | Ghi hình video demo sản phẩm và hoàn thiện báo cáo tổng kết song ngữ. | 14/08/2026 | 14/08/2026 |  |

### Kết quả đạt me

1. Script hóa hoàn toàn quy trình deploy và dọn dẹp tài nguyên AWS chỉ với một câu lệnh.
2. Hoàn tất kiểm thử end-to-end, xử lý tốt các trường hợp lỗi và tối ưu độ trễ Lambda dựa trên metric CloudWatch.
3. Đóng gói hoàn chỉnh dự án với video demo, báo cáo song ngữ và định hướng mở rộng pipeline AI qua AWS Step Functions.

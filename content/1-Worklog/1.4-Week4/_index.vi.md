---
title: "Worklog Tuần 4"
date: 2026-06-22
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4

* Tích hợp Amazon S3 làm lưu trữ chính với presigned URL.
* Cấu hình CORS và thiết lập chính sách IAM phân quyền tối thiểu.

### Các công việc trong tuần (22/06 - 26/06/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Khởi tạo S3 bucket private (ap-southeast-1), kích hoạt Block Public Access và mã hóa SSE-S3. | 22/06/2026 | 22/06/2026 | [Amazon S3](https://000057.awsstudygroup.com) |
| 3 | Lập trình hàm sinh presigned URL (upload/download) bằng `boto3` với thời hạn 15 phút và kiểm thử bằng `curl`. | 23/06/2026 | 23/06/2026 |  |
| 4 | Thiết lập cấu hình CORS cho S3 bucket hỗ trợ trình duyệt upload trực tiếp qua presigned URL. | 24/06/2026 | 24/06/2026 |  |
| 5 | Tích hợp S3 Storage vào lớp interface đã tách từ Tuần 3 mà không làm ảnh hưởng logic nghiệp vụ. | 25/06/2026 | 25/06/2026 |  |
| 6 | Tạo IAM policy chuẩn least-privilege giới hạn quyền S3 và kiểm thử các kịch bản ngoại lệ (URL hết hạn, sai key). | 26/06/2026 | 26/06/2026 |  |

### Kết quả đạt được

1. Lưu trữ file an toàn trên S3 private qua presigned URL mà không cần mở public bucket.
2. Chuyển đổi thành công sang S3 nhờ thiết kế lớp interface linh hoạt từ trước.
3. Hoàn thiện chính sách IAM phân quyền tối thiểu và xử lý tốt các lỗi.

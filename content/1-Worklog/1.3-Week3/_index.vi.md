---
title: "Worklog Tuần 3"
date: 2026-06-15
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3

* Xây dựng và chạy thử ứng dụng InsightShare tại local.
* Tách bạch module lưu trữ và AI để thuận tiện nâng cấp về sau.
* Kiểm thử các luồng chức năng cơ bản trước khi đưa lên AWS.

### Các công việc trong tuần (15/06 - 19/06/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Khởi tạo dự án FastAPI, thiết kế các endpoint upload và liệt kê file (`POST /files`, `GET /files`). | 15/06/2026 | 15/06/2026 | [FastAPI](https://fastapi.tiangolo.com/) |
| 3 | Lập trình API upload/liệt kê file, tạm thời lưu dữ liệu tại local và trả về thông tin file. | 16/06/2026 | 16/06/2026 |  |
| 4 | Xây dựng giao diện web cơ bản (HTML/JS) gồm form tải file, danh sách file và thanh tiến trình. | 17/06/2026 | 17/06/2026 |  |
| 5 | Trừu tượng hóa lớp Storage và AI bằng Abstract Base Class trong Python, sử dụng mock data cho dịch vụ AI. | 18/06/2026 | 18/06/2026 |  |
| 6 | Tái cấu trúc mã nguồn theo mô hình 3 lớp (API - Service - Storage) và viết unit test với `pytest`. | 19/06/2026 | 19/06/2026 |  |

### Kết quả đạt được

1. Hoàn thiện ứng dụng chạy local, hỗ trợ upload và xem danh sách file trên giao diện.
2. Tách lớp lưu trữ và AI rõ ràng, sẵn sàng cho việc tích hợp dịch vụ AWS.
3. Cấu trúc code chuẩn hóa theo tầng và có unit test cho chức năng lõi.

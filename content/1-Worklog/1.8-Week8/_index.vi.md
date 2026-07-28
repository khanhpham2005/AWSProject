---
title: "Worklog Tuần 8"
date: 2026-07-20
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8

* Tích hợp Amazon Cognito để quản lý xác thực người dùng.
* Phân quyền dữ liệu theo user, đảm bảo tính riêng tư cho từng tài khoản.

### Các công việc trong tuần (20/07 - 24/07/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Khởi tạo Cognito User Pool và App Client (chế độ `USER_PASSWORD_AUTH`), lưu cấu hình Pool ID và Client ID. | 20/07/2026 | 20/07/2026 | [Cognito lab](https://000081.awsstudygroup.com) |
| 3 | Tích hợp JWT Authorizer vào API Gateway, mở route OPTIONS công khai để xử lý CORS preflight. | 21/07/2026 | 21/07/2026 |  |
| 4 | Cập nhật Lambda trích xuất claim `sub` từ JWT để xác định danh tính và lọc dữ liệu theo từng user. | 22/07/2026 | 22/07/2026 |  |
| 5 | Tích hợp luồng đăng ký, xác nhận và đăng nhập trực tiếp từ frontend với `cognito-idp` mà không dùng thư viện ngoài. | 23/07/2026 | 23/07/2026 |  |
| 6 | Kiểm thử toàn bộ luồng: đăng ký → xác nhận → đăng nhập → gọi API với token (200), không token (401), và OPTIONS (200). | 24/07/2026 | 24/07/2026 | Postman |

### Kết quả đạt được

1. Hoàn thành hệ thống xác thực người dùng bằng Cognito; API Gateway bảo mật qua JWT Authorizer.
2. Bảo mật dữ liệu người dùng: Lambda tự động phân quyền và chỉ trả về file thuộc sở hữu của user tương ứng.
3. Xử lý triệt để luồng CORS preflight qua route OPTIONS, đảm bảo API chặn chính xác các request không hợp lệ.

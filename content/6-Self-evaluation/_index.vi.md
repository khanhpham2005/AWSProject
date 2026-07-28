---
title: "Tự đánh giá"
date: 2026-06-01
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

Thực tập tại **Công ty TNHH Amazon Web Services Việt Nam** (chương trình First Cloud AI Journey) từ **01/06/2026** đến **15/08/2026**.

Sản phẩm chính: **InsightShare** – ứng dụng serverless upload và chia sẻ ảnh/tài liệu trên AWS. Xây dựng bằng Python (`boto3`) kết hợp S3, Lambda, API Gateway, DynamoDB, CloudFront, IAM, CloudWatch; tài liệu viết song ngữ.

Đánh giá cá nhân theo 8 tiêu chí:

| STT | Tiêu chí | Tốt | Khá | Nhận xét |
| --- | --- | --- | --- | --- |
| 1 | **Kỹ năng chuyên môn** | x | | Áp dụng thành thạo các dịch vụ AWS cốt lõi vào dự án end-to-end. |
| 2 | **Khả năng học hỏi** | x | | Chủ động tự học công nghệ mới (Lambda, presigned URL, CloudFront) qua tài liệu & lab. |
| 3 | **Tính chủ động** | x | | Tiên phong trong thiết kế hệ thống và nghiên cứu dịch vụ phù hợp. |
| 4 | **Kỷ luật** | | x | Đảm bảo lịch lên văn phòng và nộp worklog hàng tuần đúng hạn. |
| 5 | **Giao tiếp** | x | | Báo cáo công việc rõ ràng, hoàn thiện tài liệu kỹ thuật song ngữ. |
| 6 | **Hợp tác nhóm** | | x | Hòa nhập tốt, chủ động tham vấn mentor và hỗ trợ đồng đội. |
| 7 | **Tư duy giải quyết vấn đề** | x | | Tra cứu log CloudWatch để xử lý triệt để lỗi tích hợp (CORS, IAM, cold start, S3 307, `Decimal` DynamoDB). |
| 8 | **Đóng góp dự án** | x | | Phát triển InsightShare end-to-end và mở rộng tính năng (xóa file, link hết hạn, giới hạn upload). |

### Bài học kỹ thuật

* S3 presigned URL ở Singapore yêu cầu client ép endpoint theo region và dùng Signature V4 để tránh lỗi HTTP 307.
* Lambda cache credentials trong execution environment, cần deploy/update lại function để áp dụng policy IAM mới.
* `text` là DynamoDB reserved keyword, bắt buộc dùng `ExpressionAttributeNames` khi update.
* DynamoDB trả số dạng `Decimal`, cần JSON encoder tùy chỉnh để tránh lỗi serialization với `json.dumps`.
* Tích hợp AI (Textract, Bedrock) cần cơ chế fail-soft để hệ thống hoạt động ổn định khi dịch vụ gặp sự cố.
* CloudWatch log là công cụ chẩn đoán lỗi cốt lõi cho ứng dụng serverless.

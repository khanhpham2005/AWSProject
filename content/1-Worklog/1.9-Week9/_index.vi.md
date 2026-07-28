---
title: "Worklog Tuần 9"
date: 2026-07-27
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9

* Tích hợp các dịch vụ AI để phân tích và hiểu nội dung file theo từng user.
* Sử dụng dịch vụ managed AI của AWS thay vì tự huấn luyện mô hình.

### Các công việc trong tuần (27/07 - 31/07/2026)

| Thứ | Công việc | Bắt đầu | Hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Nghiên cứu workshop AI services của FCAJ, xác định vị trí tích hợp Rekognition và Textract trong pipeline upload. | 27/07/2026 | 27/07/2026 | [AI services](https://000056.awsstudygroup.com) |
| 3 | Tích hợp Amazon Rekognition (`detect_labels`) để tự động gán nhãn nhận diện cho tệp hình ảnh. | 28/07/2026 | 28/07/2026 |  |
| 4 | Sử dụng Amazon Textract (`detect_document_text`) để trích xuất văn bản từ PDF/ảnh, đọc trực tiếp file `.txt` từ S3. | 29/07/2026 | 29/07/2026 |  |
| 5 | Phát triển endpoint `POST /files/{id}/ask` kết nối Claude trên Amazon Bedrock (`invoke_model`) để hỏi đáp/tóm tắt tài liệu. | 30/07/2026 | 30/07/2026 | [Bedrock](https://docs.aws.amazon.com/bedrock/) |
| 6 | Mở rộng IAM Role (quyền Rekognition/Textract/Bedrock), lưu nhãn và text vào DynamoDB theo owner, kiểm thử toàn bộ pipeline. | 31/07/2026 | 31/07/2026 |  |

### Kết quả đạt được

1. Tự động gắn nhãn hình ảnh (Rekognition) và trích xuất text (Textract/S3), lưu trữ dữ liệu phân tích theo từng user.
2. Hoàn thiện tính năng hỏi đáp và tóm tắt tài liệu bằng Bedrock (Claude) hỗ trợ đa ngôn ngữ, có cơ chế fail-soft chống đứt gãy luồng.
3. Lưu trữ dữ liệu AI lên DynamoDB làm nền tảng cho tính năng tìm kiếm, phân quyền IAM chuẩn least-privilege.

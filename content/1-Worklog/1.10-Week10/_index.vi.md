---
title: "Tuần 10: Tìm hiểu AWS Lambda và quản lý tài nguyên bằng AWS Systems Manager"
menuTitle: "Nhật ký tuần 10"
date: 2026-11-11
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

**Thời gian:** 12/10/2026 – 16/10/2026.

Tuần này gồm hai hướng bổ sung: thực thi tác vụ theo sự kiện với Lambda và quản lý máy chủ với Systems Manager. Các nội dung được nghiên cứu riêng. Không xem đây là bằng chứng hai dịch vụ đã được tích hợp vào CloudDocs.

## Mục tiêu trong tuần

- Hiểu function, trigger, execution role và giới hạn thực thi của Lambda.
- Hiểu điều kiện dùng Session Manager, Run Command và quản lý cấu hình.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | Tìm hiểu Lambda function, runtime và trigger. So sánh xử lý tác vụ theo sự kiện với backend chạy thường trực trên EC2. | 12/10/2026 | 12/10/2026 | [Tự động hóa với AWS Lambda](https://000022.awsfcaj.com/) |
| Thứ Ba | Đọc về execution role, timeout, memory và log. Xem xét một tác vụ xử lý sự kiện S3 ở mức ý tưởng mở rộng. | 13/10/2026 | 13/10/2026 | [Tự động hóa với AWS Lambda](https://000022.awsfcaj.com/) |
| Thứ Tư | Tìm hiểu Systems Manager và managed node. Đọc yêu cầu về SSM Agent, IAM Role và kết nối tới các endpoint dịch vụ. | 14/10/2026 | 14/10/2026 | [Quản lý hệ thống với Systems Manager](https://000031.awsfcaj.com/) |
| Thứ Năm | So sánh Session Manager với SSH và tìm hiểu Run Command. Ghi lại yêu cầu kiểm soát quyền và phạm vi máy chủ bị tác động. | 15/10/2026 | 15/10/2026 | [Truy cập máy chủ qua Session Manager](https://000058.awsfcaj.com/)<br>[Quản lý hệ thống với Systems Manager](https://000031.awsfcaj.com/) |
| Thứ Sáu | Đọc về Parameter Store, phân biệt cấu hình thông thường với dữ liệu nhạy cảm. Tổng hợp hướng ứng dụng vào vận hành CloudDocs. | 16/10/2026 | 16/10/2026 | [Quản lý hệ thống với Systems Manager](https://000031.awsfcaj.com/) |

</div>

## Tổng kết tuần

Em phân biệt Lambda là môi trường thực thi theo sự kiện, còn Systems Manager phục vụ quản lý tài nguyên và vận hành. CloudDocs hiện vẫn được trình bày theo backend trên EC2. Các ý tưởng Lambda là hướng mở rộng.

## Điểm cần làm rõ

Không phải mọi chức năng backend đều phù hợp chuyển sang Lambda. Session Manager cũng chỉ hoạt động khi máy chủ, quyền và kết nối dịch vụ đáp ứng các điều kiện cần thiết.

## Hướng học tiếp theo

[Tuần 11: Tìm hiểu Elastic Load Balancing, EC2 Auto Scaling và triển khai ứng dụng trên nhiều Availability Zone](../1.11-Week11/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Tự động hóa với AWS Lambda](https://000022.awsfcaj.com/)
- [Quản lý hệ thống với Systems Manager](https://000031.awsfcaj.com/)
- [Truy cập máy chủ qua Session Manager](https://000058.awsfcaj.com/)

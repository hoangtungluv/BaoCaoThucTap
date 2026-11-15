---
title: "Tuần 11: Tìm hiểu Elastic Load Balancing, EC2 Auto Scaling và triển khai ứng dụng trên nhiều Availability Zone"
menuTitle: "Nhật ký tuần 11"
date: 2026-11-11
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

**Thời gian:** 19/10/2026 – 23/10/2026.

Tuần này mở rộng từ một máy chủ sang kiến trúc có nhiều thành phần phục vụ. Em tìm hiểu cách phân phối lưu lượng, điều chỉnh số lượng máy chủ và giảm phụ thuộc vào một vị trí triển khai.

## Mục tiêu trong tuần

- Phân biệt cân bằng tải, mở rộng tài nguyên và tính sẵn sàng.
- Phân tích điều kiện cần khi mở rộng backend CloudDocs qua nhiều máy chủ.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | So sánh mở rộng theo chiều dọc và chiều ngang. Xác định giới hạn của phương án chỉ tăng cấu hình một EC2. | 19/10/2026 | 19/10/2026 | [Mở rộng ứng dụng với EC2 Auto Scaling](https://000006.awsfcaj.com/) |
| Thứ Ba | Tìm hiểu Application Load Balancer, listener, target group và health check. Phân tích đường đi của một yêu cầu HTTP. | 20/10/2026 | 20/10/2026 | [Xây dựng ứng dụng web có tính sẵn sàng cao](https://000101.awsfcaj.com/)<br>[Mở rộng ứng dụng với EC2 Auto Scaling](https://000006.awsfcaj.com/) |
| Thứ Tư | Đọc về launch template, Auto Scaling Group và các mức minimum, desired, maximum. Tìm hiểu chính sách mở rộng theo chỉ số. | 21/10/2026 | 21/10/2026 | [Mở rộng ứng dụng với EC2 Auto Scaling](https://000006.awsfcaj.com/) |
| Thứ Năm | Tìm hiểu bố trí tài nguyên qua nhiều Availability Zone. Phân biệt tính sẵn sàng của lớp ứng dụng với lớp cơ sở dữ liệu. | 22/10/2026 | 22/10/2026 | [Xây dựng ứng dụng web có tính sẵn sàng cao](https://000101.awsfcaj.com/)<br>[Làm quen Amazon RDS](https://000005.awsfcaj.com/) |
| Thứ Sáu | Phác thảo hướng mở rộng CloudDocs. Rà soát session, tệp cục bộ, cấu hình dùng chung và kết nối DB khi có nhiều backend. | 23/10/2026 | 23/10/2026 | [Xây dựng ứng dụng web có tính sẵn sàng cao](https://000101.awsfcaj.com/) |

</div>

## Tổng kết tuần

Em hiểu rằng thêm máy chủ chưa đủ để tạo một hệ thống sẵn sàng cao. Cần đồng thời xem xét health check, dữ liệu dùng chung và các điểm lỗi còn lại. Kiến trúc nhiều AZ trong tuần này là nội dung phân tích, không phải kết quả triển khai đã xác nhận.

## Điểm cần làm rõ

Auto Scaling không tự giải quyết mọi nút thắt hiệu năng. Nếu cơ sở dữ liệu hoặc cách quản lý trạng thái là điểm nghẽn, tăng số backend có thể không cải thiện kết quả như mong đợi.

## Hướng học tiếp theo

[Tuần 12: Tổng hợp kiến thức, liên hệ với dự án CloudDocs và hoàn thiện báo cáo thực tập](../1.12-Week12/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Mở rộng ứng dụng với EC2 Auto Scaling](https://000006.awsfcaj.com/)
- [Xây dựng ứng dụng web có tính sẵn sàng cao](https://000101.awsfcaj.com/)
- [Làm quen Amazon RDS](https://000005.awsfcaj.com/)

---
title: "Worklog tuần 4"
menuTitle: "Worklog tuần 4"
date: 2026-11-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

**Thời gian:** 31/08/2026 – 04/09/2026.

Từ kiến thức mạng, em tìm hiểu lựa chọn máy chủ để chạy ứng dụng. EC2 là nội dung chính. Lightsail được dùng làm đối tượng so sánh về cách tổ chức tài nguyên và mức độ quản lý.

## Mục tiêu trong tuần

- Hiểu AMI, instance type, EBS và các cách kết nối EC2.
- So sánh EC2 và Lightsail theo nhu cầu cấu hình, vận hành và chi phí.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | Tìm hiểu EC2 Instance, AMI và instance type. Phân biệt hệ điều hành mẫu với cấu hình CPU, bộ nhớ của máy chủ. | 31/08/2026 | 31/08/2026 | [Tổng quan Amazon EC2](https://000004.awsfcaj.com/1-introduce/) |
| Thứ Ba | Đọc về EBS, volume gốc và snapshot. Phân biệt vòng đời dữ liệu lưu trữ với vòng đời máy chủ. | 01/09/2026 | 01/09/2026 | [Tạo và quản lý EBS Snapshot](https://000004.awsfcaj.com/5-amazonec2basic/5.2-createec2snapshot/) |
| Thứ Tư | Tìm hiểu yêu cầu kết nối EC2 qua SSH hoặc Session Manager. Đối chiếu quyền truy cập, cấu hình mạng và phần mềm cần thiết. | 02/09/2026 | 02/09/2026 | [Kết nối Amazon Linux Instance](https://000004.awsfcaj.com/4-launchlinuxinstance/4.2-connectlinuxinstance/)<br>[Truy cập máy chủ qua Session Manager](https://000058.awsfcaj.com/) |
| Thứ Năm | Đọc tổng quan Lightsail và các gói tài nguyên. So sánh với cách chọn riêng từng thành phần trong EC2. | 03/09/2026 | 03/09/2026 | [Làm quen Amazon Lightsail](https://000045.awsfcaj.com/) |
| Thứ Sáu | Phân tích nhu cầu chạy backend CloudDocs. Ghi lý do EC2 phù hợp khi cần chủ động cấu hình mạng, IAM Role và kết nối dịch vụ. | 04/09/2026 | 04/09/2026 | [Giới thiệu Amazon EC2](https://000004.awsfcaj.com/)<br>[IAM Role cho EC2](https://000048.awsfcaj.com/) |

</div>

## Tổng kết tuần

Em phân biệt được cấu hình máy chủ, ổ đĩa và kết nối mạng là các phần cần xem xét riêng. Việc chọn EC2 hay Lightsail phụ thuộc yêu cầu ứng dụng và khả năng vận hành, không chỉ dựa trên giá gói dịch vụ.

## Điểm cần làm rõ

Dừng EC2 không đồng nghĩa toàn bộ chi phí liên quan kết thúc. Cần xem riêng các tài nguyên còn giữ như EBS, snapshot và địa chỉ IP công khai.

## Hướng học tiếp theo

[Tuần 5: Tìm hiểu Amazon S3 và các hình thức lưu trữ trên AWS](../1.5-Week5/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Tổng quan Amazon EC2](https://000004.awsfcaj.com/1-introduce/)
- [Tạo và quản lý EBS Snapshot](https://000004.awsfcaj.com/5-amazonec2basic/5.2-createec2snapshot/)
- [Kết nối Amazon Linux Instance](https://000004.awsfcaj.com/4-launchlinuxinstance/4.2-connectlinuxinstance/)
- [Truy cập máy chủ qua Session Manager](https://000058.awsfcaj.com/)
- [Làm quen Amazon Lightsail](https://000045.awsfcaj.com/)
- [Giới thiệu Amazon EC2](https://000004.awsfcaj.com/)
- [IAM Role cho EC2](https://000048.awsfcaj.com/)

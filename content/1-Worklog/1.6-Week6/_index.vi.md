---
title: "Worklog tuần 6"
menuTitle: "Worklog tuần 6"
date: 2026-11-11
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

**Thời gian:** 14/09/2026 – 18/09/2026.

Sau phần lưu tệp, em tìm hiểu cách lưu dữ liệu nghiệp vụ. Tuần này lấy RDS MySQL làm trọng tâm và dùng DynamoDB để so sánh cách mô hình hóa dữ liệu, truy vấn và lựa chọn cơ sở dữ liệu.

## Mục tiêu trong tuần

- Hiểu kết nối RDS, bảo vệ truy cập và các khái niệm sao lưu cơ bản.
- Phân biệt mô hình quan hệ với mô hình key-value/document của DynamoDB.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | Tìm hiểu RDS, DB instance, engine và endpoint. Phân biệt dịch vụ quản lý cơ sở dữ liệu với việc tự cài MySQL trên máy chủ. | 14/09/2026 | 14/09/2026 | [Tổng quan Amazon RDS](https://000005.awsfcaj.com/1-introduce/) |
| Thứ Ba | Đọc về DB subnet group, Security Group và TLS. Phân tích điều kiện để backend kết nối RDS. | 15/09/2026 | 15/09/2026 | [Chuẩn bị mạng và quyền truy cập RDS](https://000005.awsfcaj.com/2-prerequiste/)<br>[Tổng quan RDS và mã hóa kết nối](https://000005.awsfcaj.com/1-introduce/) |
| Thứ Tư | Tìm hiểu automated backup, snapshot, Multi-AZ và read replica. Phân biệt phục hồi dữ liệu, tính sẵn sàng và mở rộng đọc. | 16/09/2026 | 16/09/2026 | [Sao lưu và phục hồi RDS](https://000005.awsfcaj.com/6-backup/)<br>[Tổng quan Amazon RDS](https://000005.awsfcaj.com/1-introduce/) |
| Thứ Năm | Đọc tổng quan DynamoDB: table, item, partition key, sort key và index. Tìm hiểu cách thiết kế theo mẫu truy cập. | 17/09/2026 | 17/09/2026 | [Làm quen Amazon DynamoDB](https://000060.awsfcaj.com/) |
| Thứ Sáu | So sánh hai lựa chọn với dữ liệu người dùng, tài liệu và chia sẻ của CloudDocs. Giải thích lý do tiếp tục dùng MySQL cho mô hình hiện tại. | 18/09/2026 | 18/09/2026 | [Làm quen Amazon RDS](https://000005.awsfcaj.com/1-introduce/)<br>[Làm quen Amazon DynamoDB](https://000060.awsfcaj.com/) |

</div>

## Tổng kết tuần

Em nhận thấy lựa chọn cơ sở dữ liệu cần xuất phát từ quan hệ dữ liệu và nhu cầu truy vấn. DynamoDB là nội dung so sánh mở rộng. Cơ sở dữ liệu trong phương án CloudDocs vẫn là MySQL.

## Điểm cần làm rõ

Multi-AZ không thay thế sao lưu. Cần phân biệt khả năng duy trì dịch vụ khi có sự cố hạ tầng với khả năng phục hồi dữ liệu bị sửa hoặc xóa nhầm.

## Hướng học tiếp theo

[Tuần 7: Tìm hiểu AWS CLI, AWS CloudShell và sử dụng IAM Role](../1.7-Week7/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Tổng quan Amazon RDS](https://000005.awsfcaj.com/1-introduce/)
- [Chuẩn bị mạng và quyền truy cập RDS](https://000005.awsfcaj.com/2-prerequiste/)
- [Sao lưu và phục hồi RDS](https://000005.awsfcaj.com/6-backup/)
- [Làm quen Amazon DynamoDB](https://000060.awsfcaj.com/)

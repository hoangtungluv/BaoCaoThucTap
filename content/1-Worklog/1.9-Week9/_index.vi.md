---
title: "Worklog tuần 9"
menuTitle: "Worklog Tuần 9"
date: 2026-11-11
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

**Thời gian:** 05/10/2026 – 09/10/2026.

Sau khi tìm hiểu các thành phần ứng dụng, em chuyển sang câu hỏi làm thế nào nhận biết hệ thống đang hoạt động bình thường. CloudWatch được nghiên cứu qua metrics, logs, alarms và cách đối chiếu dấu hiệu sự cố.

## Mục tiêu trong tuần

- Phân biệt metric, log, dashboard và alarm.
- Xác định thông tin giám sát phù hợp cho EC2, RDS và backend CloudDocs.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | Tìm hiểu metric, namespace và dimension. Đọc ví dụ theo dõi CPU EC2 và kết nối cơ sở dữ liệu RDS. | 05/10/2026 | 05/10/2026 | [Xem các chỉ số CloudWatch](https://000036.awsfcaj.com/3-cloudwatchmetric/3.1-view/)<br>[Chỉ số EC2 mặc định và CloudWatch](https://000032.awsfcaj.com/4-cloudwatch-intro/) |
| Thứ Ba | Đọc về CloudWatch Logs, log group, log stream và retention. Xác định loại nhật ký ứng dụng cần thu thập. | 06/10/2026 | 06/10/2026 | [CloudWatch Logs, log group và log stream](https://000036.awsfcaj.com/4-cloudwatchlogs/4.1-logs/) |
| Thứ Tư | Tìm hiểu CloudWatch Agent. Phân biệt chỉ số EC2 có sẵn với chỉ số hệ điều hành như bộ nhớ cần cơ chế thu thập bổ sung. | 07/10/2026 | 07/10/2026 | [Cài CloudWatch Agent để thu thập chỉ số hệ điều hành](https://000032.awsfcaj.com/5-install-cloudwatch-agent/) |
| Thứ Năm | Đọc cách xác định threshold, evaluation period và missing data cho alarm. Tìm hiểu kết nối thông báo với Amazon SNS. | 08/10/2026 | 08/10/2026 | [Tạo CloudWatch Alarm và thông báo](https://000036.awsfcaj.com/5-cloudwatchalarm/) |
| Thứ Sáu | Xây dựng cách tiếp cận tình huống backend phản hồi chậm trên giấy: đối chiếu thời điểm lỗi, CPU, kết nối DB và log ứng dụng. | 09/10/2026 | 09/10/2026 | [Xem các chỉ số CloudWatch](https://000036.awsfcaj.com/3-cloudwatchmetric/3.1-view/)<br>[CloudWatch Logs, log group và log stream](https://000036.awsfcaj.com/4-cloudwatchlogs/4.1-logs/) |

</div>

## Tổng kết tuần

Em hiểu rằng một chỉ số riêng lẻ thường chưa đủ để kết luận nguyên nhân sự cố. Cần đối chiếu metrics với log theo cùng khoảng thời gian, đồng thời xác định ngưỡng cảnh báo theo đặc điểm ứng dụng.

## Điểm cần làm rõ

Không ghi mật khẩu, access token hoặc presigned URL vào log. Cũng cần cân nhắc thời gian lưu log và mức thu thập để kiểm soát chi phí giám sát.

## Hướng học tiếp theo

[Tuần 10: Tìm hiểu AWS Lambda và quản lý tài nguyên bằng AWS Systems Manager](../1.10-Week10/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Xem các chỉ số CloudWatch](https://000036.awsfcaj.com/3-cloudwatchmetric/3.1-view/)
- [Chỉ số EC2 mặc định và CloudWatch](https://000032.awsfcaj.com/4-cloudwatch-intro/)
- [CloudWatch Logs, log group và log stream](https://000036.awsfcaj.com/4-cloudwatchlogs/4.1-logs/)
- [Cài CloudWatch Agent để thu thập chỉ số hệ điều hành](https://000032.awsfcaj.com/5-install-cloudwatch-agent/)
- [Tạo CloudWatch Alarm và thông báo](https://000036.awsfcaj.com/5-cloudwatchalarm/)

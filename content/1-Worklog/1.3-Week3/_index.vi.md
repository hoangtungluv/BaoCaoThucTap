---
title: "Tuần 3: Tìm hiểu Amazon VPC và các thành phần mạng"
menuTitle: "Nhật ký tuần 3"
date: 2026-11-11
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

**Thời gian:** 24/08/2026 – 28/08/2026.

Tuần này tìm hiểu đường đi của lưu lượng trong AWS, từ không gian địa chỉ mạng đến các lớp kiểm soát truy cập. Mục tiêu là đọc được sơ đồ mạng cơ bản cho một ứng dụng có máy chủ và cơ sở dữ liệu.

## Mục tiêu trong tuần

- Hiểu quan hệ giữa VPC, CIDR, subnet và Availability Zone.
- Phân biệt định tuyến với kiểm soát truy cập bằng Security Group và Network ACL.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | Tìm hiểu VPC và CIDR. Đọc ví dụ chia không gian địa chỉ thành các subnet không chồng lấn. | 24/08/2026 | 24/08/2026 | [Amazon VPC và các thành phần mạng](https://000003.awsfcaj.com/1-introduce/)<br>[Subnet trong VPC](https://000003.awsfcaj.com/1-introduce/1.1-subnets/) |
| Thứ Ba | Phân biệt public subnet và private subnet theo cấu hình định tuyến. Tìm hiểu quan hệ subnet với Availability Zone. | 25/08/2026 | 25/08/2026 | [Subnet trong VPC](https://000003.awsfcaj.com/1-introduce/1.1-subnets/) |
| Thứ Tư | Tìm hiểu Route Table, Internet Gateway và NAT Gateway. Phân tích đường đi ra Internet của các nhóm tài nguyên. | 26/08/2026 | 26/08/2026 | [Route Table](https://000003.awsfcaj.com/1-introduce/1.2-routetable/)<br>[NAT Gateway](https://000003.awsfcaj.com/1-introduce/1.4-natgateway/) |
| Thứ Năm | So sánh Security Group và Network ACL về phạm vi áp dụng, trạng thái kết nối và cách xử lý quy tắc. | 27/08/2026 | 27/08/2026 | [Security Group](https://000003.awsfcaj.com/2-firewallinvpc/2.1-securitygroup/)<br>[Network ACL](https://000003.awsfcaj.com/2-firewallinvpc/2.2-networkacls/) |
| Thứ Sáu | Đọc sơ đồ bố trí máy chủ ứng dụng và cơ sở dữ liệu. Ghi lại những đường kết nối cần cho phép và những đường cần hạn chế. | 28/08/2026 | 28/08/2026 | [Amazon VPC và các thành phần mạng](https://000003.awsfcaj.com/1-introduce/)<br>[Làm quen Amazon RDS](https://000005.awsfcaj.com/) |

</div>

## Tổng kết tuần

Em hiểu rằng kết nối thành công phụ thuộc nhiều lớp: địa chỉ, định tuyến, quyền truy cập mạng và cấu hình dịch vụ. Sơ đồ mạng giúp kiểm tra từng lớp thay vì thay đổi nhiều thiết lập cùng lúc.

## Điểm cần làm rõ

Đặt tài nguyên trong public subnet chưa đủ để bảo đảm truy cập từ Internet. Còn phải xem địa chỉ công khai, đường định tuyến và các quy tắc cho phép kết nối.

## Hướng học tiếp theo

[Tuần 4: Tìm hiểu Amazon EC2 và so sánh với Amazon Lightsail](../1.4-Week4/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Amazon VPC và các thành phần mạng](https://000003.awsfcaj.com/1-introduce/)
- [Subnet trong VPC](https://000003.awsfcaj.com/1-introduce/1.1-subnets/)
- [Route Table](https://000003.awsfcaj.com/1-introduce/1.2-routetable/)
- [NAT Gateway](https://000003.awsfcaj.com/1-introduce/1.4-natgateway/)
- [Security Group](https://000003.awsfcaj.com/2-firewallinvpc/2.1-securitygroup/)
- [Network ACL](https://000003.awsfcaj.com/2-firewallinvpc/2.2-networkacls/)
- [Làm quen Amazon RDS](https://000005.awsfcaj.com/)

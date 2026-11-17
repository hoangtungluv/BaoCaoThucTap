---
title: "Worklog tuần 7"
menuTitle: "Worklog Tuần 7"
date: 2026-11-11
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

**Thời gian:** 21/09/2026 – 25/09/2026.

Tuần này chuyển từ việc nhận biết dịch vụ sang cách tương tác với tài nguyên bằng dòng lệnh. Em quay lại IAM Role trong ngữ cảnh sử dụng thông tin xác thực và truy cập dịch vụ từ môi trường làm việc hoặc EC2.

## Mục tiêu trong tuần

- Hiểu vai trò AWS CLI, profile, Region và môi trường AWS CloudShell.
- Phân biệt thông tin xác thực dài hạn với thông tin xác thực tạm thời từ role.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | Đọc cấu trúc lệnh AWS CLI và cách xem trợ giúp. Tìm hiểu ảnh hưởng của Region và định dạng đầu ra. | 21/09/2026 | 21/09/2026 | [Làm quen AWS CLI](https://000011.awsfcaj.com/) |
| Thứ Ba | Tìm hiểu profile và nguồn thông tin xác thực. Phân tích lệnh aws sts get-caller-identity để nhận biết danh tính đang sử dụng. | 22/09/2026 | 22/09/2026 | [Profile và thông tin xác thực AWS CLI](https://000011.awsfcaj.com/)<br>[Kiểm tra danh tính bằng AWS STS trong CloudShell](https://000037.awsfcaj.com/3-cloudformationbasic/3.1-launchawscloudshell/) |
| Thứ Tư | Tìm hiểu AWS CloudShell, môi trường dòng lệnh trên trình duyệt và phạm vi quyền kế thừa từ phiên đăng nhập. | 23/09/2026 | 23/09/2026 | [Làm quen AWS CloudShell](https://000049.awsfcaj.com/) |
| Thứ Năm | Đọc về IAM Role cho EC2 và instance profile. Đối chiếu cách ứng dụng lấy thông tin xác thực tạm thời thay vì ghi access key vào mã nguồn. | 24/09/2026 | 24/09/2026 | [IAM Role cho EC2](https://000048.awsfcaj.com/) |
| Thứ Sáu | Phân tích các lệnh tra cứu tài nguyên và tình huống lỗi. Tổng hợp cách kiểm tra danh tính, Region và quyền trước khi thay đổi cấu hình. | 25/09/2026 | 25/09/2026 | [Xử lý lỗi AWS CLI](https://000011.awsfcaj.com/10-troubleshoot/)<br>[AWS CLI với IAM](https://000011.awsfcaj.com/7-iam/) |

</div>

## Tổng kết tuần

Em hiểu rằng cùng một lệnh có thể cho kết quả khác nhau khi thay đổi danh tính, Region hoặc tài khoản. Kiến thức IAM của tuần 2 được liên hệ với tình huống ứng dụng trên EC2 cần truy cập S3.

## Điểm cần làm rõ

CloudShell là môi trường thực thi lệnh, không phải cách vượt qua giới hạn quyền IAM. Trước khi chạy lệnh thay đổi tài nguyên, cần hiểu lệnh đang tác động vào tài khoản và Region nào.

## Hướng học tiếp theo

[Tuần 8: Tìm hiểu Amazon Cognito, xác thực người dùng và kiểm soát truy cập bằng token](../1.8-Week8/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Làm quen AWS CLI](https://000011.awsfcaj.com/)
- [Kiểm tra danh tính bằng AWS STS trong CloudShell](https://000037.awsfcaj.com/3-cloudformationbasic/3.1-launchawscloudshell/)
- [Làm quen AWS CloudShell](https://000049.awsfcaj.com/)
- [IAM Role cho EC2](https://000048.awsfcaj.com/)
- [Xử lý lỗi AWS CLI](https://000011.awsfcaj.com/10-troubleshoot/)
- [AWS CLI với IAM](https://000011.awsfcaj.com/7-iam/)

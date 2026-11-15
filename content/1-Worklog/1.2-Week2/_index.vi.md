---
title: "Tuần 2: Tìm hiểu AWS IAM và quản lý quyền truy cập"
menuTitle: "Nhật ký tuần 2"
date: 2026-11-11
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

**Thời gian:** 17/08/2026 – 21/08/2026.

Sau khi làm quen với tài khoản AWS, em chuyển sang câu hỏi ai được phép thực hiện thao tác nào trên tài nguyên. Tuần này tập trung vào các thành phần IAM và cách đọc quyền truy cập.

## Mục tiêu trong tuần

- Phân biệt IAM User, Group, Policy và Role.
- Hiểu nguyên tắc quyền tối thiểu và cách tiếp cận lỗi AccessDenied.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | Tìm hiểu IAM User và IAM Group. Phân biệt danh tính sử dụng với nhóm dùng để tổ chức quyền. | 17/08/2026 | 17/08/2026 | [IAM Group và IAM User](https://000002.awsfcaj.com/1-introduction/1.1-group-user/) |
| Thứ Ba | Đọc cấu trúc IAM Policy, tập trung vào Effect, Action, Resource và Condition. Phân tích các ví dụ cấp quyền. | 18/08/2026 | 18/08/2026 | [IAM Policy](https://000002.awsfcaj.com/1-introduction/1.2-iam-policy/) |
| Thứ Tư | Tìm hiểu IAM Role, trust policy và thông tin xác thực tạm thời. Phân biệt quyền của role với đối tượng được nhận role. | 19/08/2026 | 19/08/2026 | [IAM Role](https://000002.awsfcaj.com/1-introduction/1.3-iam-role/) |
| Thứ Năm | Đọc nguyên tắc đánh giá quyền và vai trò của explicit deny. Đối chiếu các tình huống cho phép hoặc từ chối truy cập. | 20/08/2026 | 20/08/2026 | [IAM Policy](https://000002.awsfcaj.com/1-introduction/1.2-iam-policy/)<br>[Quản lý quyền truy cập với IAM](https://000002.awsfcaj.com/) |
| Thứ Sáu | Tổng hợp cách phân tích AccessDenied: xác định danh tính, thao tác, tài nguyên và các chính sách liên quan. | 21/08/2026 | 21/08/2026 | [Chuyển đổi IAM Role](https://000002.awsfcaj.com/4-switch-roles/)<br>[IAM Policy](https://000002.awsfcaj.com/1-introduction/1.2-iam-policy/) |

</div>

## Tổng kết tuần

Em phân biệt được việc tổ chức người dùng với việc cấp quyền. Khi đọc một cấu hình IAM, cần xem cả quyền thực hiện thao tác và điều kiện để danh tính có thể sử dụng quyền đó.

## Điểm cần làm rõ

Không nên xử lý lỗi truy cập bằng cách cấp AdministratorAccess ngay lập tức. Cần xác định thao tác bị thiếu hoặc điều kiện từ chối trước khi đề xuất điều chỉnh quyền.

## Hướng học tiếp theo

[Tuần 3: Tìm hiểu Amazon VPC và các thành phần mạng](../1.3-Week3/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [IAM Group và IAM User](https://000002.awsfcaj.com/1-introduction/1.1-group-user/)
- [IAM Policy](https://000002.awsfcaj.com/1-introduction/1.2-iam-policy/)
- [IAM Role](https://000002.awsfcaj.com/1-introduction/1.3-iam-role/)
- [Quản lý quyền truy cập với IAM](https://000002.awsfcaj.com/)
- [Chuyển đổi IAM Role](https://000002.awsfcaj.com/4-switch-roles/)

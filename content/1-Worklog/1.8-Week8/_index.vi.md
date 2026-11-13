---
title: "Tuần 8: Tìm hiểu Amazon Cognito, xác thực người dùng và kiểm soát truy cập bằng token"
menuTitle: "Nhật ký tuần 8"
date: 2026-11-11
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

**Thời gian:** 28/09/2026–02/10/2026.

Tuần này tập trung vào danh tính người dùng của ứng dụng. Em phân biệt đăng nhập bằng Cognito với quyền thao tác tài liệu do backend CloudDocs kiểm soát.

## Mục tiêu trong tuần

- Hiểu User Pool, App Client và luồng Authorization Code với PKCE.
- Phân biệt ID Token, Access Token, Refresh Token và kiểm tra quyền nghiệp vụ.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | Tìm hiểu User Pool, App Client và trạng thái người dùng. Phân biệt người dùng ứng dụng với IAM User. | 28/09/2026 | 28/09/2026 | [Xác thực liên ứng dụng với Cognito](https://000141.awsfcaj.com/) |
| Thứ Ba | Đọc về trang đăng nhập, callback URL và logout URL. Phân tích luồng Authorization Code kết hợp PKCE cho ứng dụng web. | 29/09/2026 | 29/09/2026 | [Triển khai và kiểm tra Cognito](https://000141.awsfcaj.com/4-app-configuration/) |
| Thứ Tư | So sánh ID Token, Access Token và Refresh Token theo mục đích sử dụng, thời hạn và cách làm mới phiên. | 30/09/2026 | 30/09/2026 | [Phân tích mã nguồn tích hợp Cognito](https://000141.awsfcaj.com/3-note-code/) |
| Thứ Năm | Tìm hiểu kiểm tra chữ ký JWT, issuer, hạn sử dụng, token_use và thông tin ứng dụng phù hợp từng loại token. | 01/10/2026 | 01/10/2026 | [Phân tích mã nguồn tích hợp Cognito](https://000141.awsfcaj.com/3-note-code/) |
| Thứ Sáu | Liên hệ các tình huống token thiếu, hết hạn hoặc người dùng không có quyền tài liệu. Phân biệt lỗi xác thực với lỗi phân quyền. | 02/10/2026 | 02/10/2026 | [Triển khai và kiểm tra Cognito](https://000141.awsfcaj.com/4-app-configuration/)<br>[Phân tích mã nguồn tích hợp Cognito](https://000141.awsfcaj.com/3-note-code/) |

</div>

## Tổng kết tuần

Em phân biệt được việc xác định danh tính người dùng với việc quyết định người dùng được thao tác trên tài liệu nào. Token hợp lệ là một điều kiện đầu vào. Backend vẫn cần kiểm tra quyền sở hữu, chia sẻ và trạng thái tài khoản theo nghiệp vụ.

## Điểm cần làm rõ

Giải mã nội dung JWT chưa đủ để tin cậy token. Cần xác minh chữ ký và các claim phù hợp. Thao tác đăng xuất cũng không nên được hiểu là mọi token đã phát hành lập tức mất hiệu lực ở mọi hệ thống kiểm tra.

## Hướng học tiếp theo

[Tuần 9: Tìm hiểu Amazon CloudWatch và giám sát hệ thống](../1.9-Week9/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Xác thực liên ứng dụng với Cognito](https://000141.awsfcaj.com/)
- [Triển khai và kiểm tra Cognito](https://000141.awsfcaj.com/4-app-configuration/)
- [Phân tích mã nguồn tích hợp Cognito](https://000141.awsfcaj.com/3-note-code/)

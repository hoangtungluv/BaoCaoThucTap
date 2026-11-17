---
title: "Worklog tuần 8"
menuTitle: "Worklog Tuần 8"
date: 2026-11-11
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

**Thời gian:** 28/09/2026 – 02/10/2026.

Tuần này tập trung vào danh tính người dùng của ứng dụng. Em phân biệt đăng nhập bằng Cognito với quyền thao tác tài liệu do backend CloudDocs kiểm soát.

## Mục tiêu trong tuần

- Hiểu User Pool, App Client và cách tích hợp Cognito vào ứng dụng web.
- Phân biệt ID Token, Access Token, Refresh Token và kiểm tra quyền nghiệp vụ.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | Tìm hiểu User Pool, App Client và trạng thái người dùng. Phân biệt người dùng ứng dụng với IAM User. | 28/09/2026 | 28/09/2026 | [Tạo Cognito User Pool và App Client](https://000081.awsfcaj.com/2-create-user-pool/) |
| Thứ Ba | Tìm hiểu cách tích hợp Cognito User Pool vào ứng dụng web. Đối chiếu cấu hình User Pool ID, App Client ID và Region trong ứng dụng. | 29/09/2026 | 29/09/2026 | [Tích hợp Cognito vào ứng dụng SPA](https://000055.awsfcaj.com/4-configure-aaa/4.1-add-authentication-with-cognito/) |
| Thứ Tư | So sánh ID Token, Access Token và Refresh Token theo mục đích sử dụng, thời hạn và cách làm mới phiên. | 30/09/2026 | 30/09/2026 | [Phân biệt các token khi đăng nhập bằng Cognito](https://000081.awsfcaj.com/3-create-api-and-lambda-function/) |
| Thứ Năm | Tìm hiểu Cognito Authorizer trên API Gateway. Đọc cách lấy token từ header Authorization và sử dụng claims để nhận biết người dùng gọi API. | 01/10/2026 | 01/10/2026 | [Bảo vệ API bằng Cognito Authorizer](https://000117.awsfcaj.com/6-identity/6.8-authorizer/) |
| Thứ Sáu | Liên hệ các tình huống token thiếu, hết hạn hoặc người dùng không có quyền tài liệu. Phân biệt lỗi xác thực với lỗi phân quyền. | 02/10/2026 | 02/10/2026 | [Xác thực API và phản hồi khi chưa được phép](https://000055.awsfcaj.com/4-configure-aaa/4.2-setup-authentication/)<br>[Đăng nhập Cognito và phân biệt các token](https://000081.awsfcaj.com/3-create-api-and-lambda-function/) |

</div>

## Tổng kết tuần

Em phân biệt được việc xác định danh tính người dùng với việc quyết định người dùng được thao tác trên tài liệu nào. Token hợp lệ là một điều kiện đầu vào. Backend vẫn cần kiểm tra quyền sở hữu, chia sẻ và trạng thái tài khoản theo nghiệp vụ.

## Điểm cần làm rõ

Giải mã nội dung JWT chưa đủ để tin cậy token. Cần xác minh chữ ký và các claim phù hợp. Thao tác đăng xuất cũng không nên được hiểu là mọi token đã phát hành lập tức mất hiệu lực ở mọi hệ thống kiểm tra.

## Hướng học tiếp theo

[Tuần 9: Tìm hiểu Amazon CloudWatch và giám sát hệ thống](../1.9-Week9/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Tạo Cognito User Pool và App Client](https://000081.awsfcaj.com/2-create-user-pool/)
- [Tích hợp Cognito vào ứng dụng SPA](https://000055.awsfcaj.com/4-configure-aaa/4.1-add-authentication-with-cognito/)
- [Phân biệt các token khi đăng nhập bằng Cognito](https://000081.awsfcaj.com/3-create-api-and-lambda-function/)
- [Bảo vệ API bằng Cognito Authorizer](https://000117.awsfcaj.com/6-identity/6.8-authorizer/)
- [Xác thực API và phản hồi khi chưa được phép](https://000055.awsfcaj.com/4-configure-aaa/4.2-setup-authentication/)

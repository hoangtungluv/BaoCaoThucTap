---
title: "Tuần 5: Tìm hiểu Amazon S3 và các hình thức lưu trữ trên AWS"
menuTitle: "Nhật ký tuần 5"
date: 2026-11-11
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

**Thời gian:** 07/09/2026 – 11/09/2026.

Tuần này tập trung vào cách lưu tệp cho ứng dụng quản lý tài liệu. Em tìm hiểu S3 và phân biệt object storage với lưu trữ khối, lưu trữ tệp trước khi liên hệ với CloudDocs.

## Mục tiêu trong tuần

- Hiểu bucket, object, key và lựa chọn hình thức lưu trữ.
- Hiểu bảo vệ bucket, CORS và luồng truyền tệp qua presigned URL.

## Nội dung công việc

<div class="worklog-table" tabindex="0" role="region" aria-label="Bảng nhật ký công việc. Cuộn ngang để xem đủ các cột.">

| Thứ | Nội dung tìm hiểu và tổng hợp | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ Hai | So sánh object storage, block storage và file storage. Xác định vai trò cơ bản của S3, EBS và EFS. | 07/09/2026 | 07/09/2026 | [Lưu trữ website tĩnh trên Amazon S3](https://000057.awsfcaj.com/)<br>[Tạo và quản lý EBS Snapshot](https://000004.awsfcaj.com/5-amazonec2basic/5.2-createec2snapshot/) |
| Thứ Ba | Tìm hiểu bucket, object key, metadata và Region. Đọc cách tổ chức tệp theo prefix trong S3. | 08/09/2026 | 08/09/2026 | [Lưu trữ website tĩnh trên Amazon S3](https://000057.awsfcaj.com/) |
| Thứ Tư | Đọc về Block Public Access, bucket policy và mã hóa. Phân biệt kiểm soát truy cập với bảo vệ dữ liệu lưu trữ. | 09/09/2026 | 09/09/2026 | [S3 Block Public Access](https://000069.awsfcaj.com/6-s3pba/)<br>[Mã hóa SSE-S3](https://000069.awsfcaj.com/4-requiresse/) |
| Thứ Năm | Tìm hiểu presigned URL và CORS. Phân tích luồng trình duyệt nhận URL từ backend rồi truyền tệp trực tiếp tới S3. | 10/09/2026 | 10/09/2026 | [AWS CLI với Amazon S3](https://000011.awsfcaj.com/5-s3/)<br>[Thực hành bảo mật Amazon S3](https://000069.awsfcaj.com/) |
| Thứ Sáu | Tìm hiểu Versioning, Lifecycle và các nhóm chi phí. Liên hệ việc lưu tệp trên S3 với metadata trong cơ sở dữ liệu CloudDocs. | 11/09/2026 | 11/09/2026 | [Lưu trữ website tĩnh trên Amazon S3](https://000057.awsfcaj.com/)<br>[Thực hành bảo mật Amazon S3](https://000069.awsfcaj.com/) |

</div>

## Tổng kết tuần

Em hiểu sự khác nhau giữa tệp trên S3 và bản ghi mô tả tệp trong cơ sở dữ liệu. Với CloudDocs, quyền tải lên hoặc tải xuống cần được backend kiểm tra trước khi cấp URL truy cập có thời hạn.

## Điểm cần làm rõ

CORS không thay thế cơ chế phân quyền. Một cấu hình CORS phù hợp không tự cấp quyền đọc hoặc ghi vào bucket.

## Hướng học tiếp theo

[Tuần 6: Tìm hiểu Amazon RDS và so sánh với Amazon DynamoDB](../1.6-Week6/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Lưu trữ website tĩnh trên Amazon S3](https://000057.awsfcaj.com/)
- [Tạo và quản lý EBS Snapshot](https://000004.awsfcaj.com/5-amazonec2basic/5.2-createec2snapshot/)
- [S3 Block Public Access](https://000069.awsfcaj.com/6-s3pba/)
- [Mã hóa SSE-S3](https://000069.awsfcaj.com/4-requiresse/)
- [AWS CLI với Amazon S3](https://000011.awsfcaj.com/5-s3/)
- [Thực hành bảo mật Amazon S3](https://000069.awsfcaj.com/)

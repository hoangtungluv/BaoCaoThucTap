---
title: "Worklog tuần 5"
menuTitle: "Worklog Tuần 5"
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
| Thứ Hai | So sánh object storage, block storage và file storage. Xác định vai trò cơ bản của S3, EBS và EFS. | 07/09/2026 | 07/09/2026 | [Tổng quan Amazon S3 và các lớp lưu trữ](https://000057.awsfcaj.com/1-introduce/)<br>[Lưu trữ EBS và Instance Store trên EC2](https://000004.awsfcaj.com/1-introduce/)<br>[Tổng quan Amazon EFS](https://000068.awsfcaj.com/4-efsstorageperformance/) |
| Thứ Ba | Tìm hiểu bucket, object key, metadata và Region. Đọc cách tổ chức tệp theo prefix trong S3. | 08/09/2026 | 08/09/2026 | [Tổng quan Amazon S3 và các lớp lưu trữ](https://000057.awsfcaj.com/1-introduce/) |
| Thứ Tư | Đọc về Block Public Access, bucket policy và mã hóa. Phân biệt kiểm soát truy cập với bảo vệ dữ liệu lưu trữ. | 09/09/2026 | 09/09/2026 | [S3 Block Public Access](https://000069.awsfcaj.com/6-s3pba/)<br>[Mã hóa SSE-S3](https://000069.awsfcaj.com/4-requiresse/) |
| Thứ Năm | Tìm hiểu presigned URL và CORS. Phân tích luồng trình duyệt nhận URL từ backend rồi truyền tệp trực tiếp tới S3. | 10/09/2026 | 10/09/2026 | [Chia sẻ dữ liệu S3 bằng presigned URL](https://000033.awsfcaj.com/6-demo/)<br>[CORS và các thực hành tốt với S3](https://000057.awsfcaj.com/12-notes/) |
| Thứ Sáu | Tìm hiểu Versioning, Lifecycle và các nhóm chi phí. Liên hệ việc lưu tệp trên S3 với metadata trong cơ sở dữ liệu CloudDocs. | 11/09/2026 | 11/09/2026 | [S3 Versioning và chi phí lưu phiên bản](https://000057.awsfcaj.com/8-versioning/)<br>[CORS và các thực hành tốt với S3](https://000057.awsfcaj.com/12-notes/) |

</div>

## Tổng kết tuần

Em hiểu sự khác nhau giữa tệp trên S3 và bản ghi mô tả tệp trong cơ sở dữ liệu. Với CloudDocs, quyền tải lên hoặc tải xuống cần được backend kiểm tra trước khi cấp URL truy cập có thời hạn.

## Điểm cần làm rõ

CORS không thay thế cơ chế phân quyền. Một cấu hình CORS phù hợp không tự cấp quyền đọc hoặc ghi vào bucket.

## Hướng học tiếp theo

[Tuần 6: Tìm hiểu Amazon RDS và so sánh với Amazon DynamoDB](../1.6-Week6/).

## Tài liệu tham khảo

- [Cloud Journey — Danh mục tài liệu](https://cloudjourney.awsfcaj.com/)
- [Tổng quan Amazon S3 và các lớp lưu trữ](https://000057.awsfcaj.com/1-introduce/)
- [Lưu trữ EBS và Instance Store trên EC2](https://000004.awsfcaj.com/1-introduce/)
- [Tổng quan Amazon EFS](https://000068.awsfcaj.com/4-efsstorageperformance/)
- [S3 Block Public Access](https://000069.awsfcaj.com/6-s3pba/)
- [Mã hóa SSE-S3](https://000069.awsfcaj.com/4-requiresse/)
- [Chia sẻ dữ liệu S3 bằng presigned URL](https://000033.awsfcaj.com/6-demo/)
- [CORS và các thực hành tốt với S3](https://000057.awsfcaj.com/12-notes/)
- [S3 Versioning và chi phí lưu phiên bản](https://000057.awsfcaj.com/8-versioning/)

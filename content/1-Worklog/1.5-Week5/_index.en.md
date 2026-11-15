---
title: "Week 5: Studying Amazon S3 and AWS storage options"
menuTitle: "Week 5 worklog"
date: 2026-11-11
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

**Period:** 07/09/2026 – 11/09/2026.

This week focuses on file storage for a document management application. I study S3 and distinguish object, block and file storage before relating the concepts to CloudDocs.

## Weekly objectives

- Understand buckets, objects, keys and storage-model selection.
- Understand bucket protection, CORS and presigned-URL file transfers.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Compare object, block and file storage. Identify the basic roles of S3, EBS and EFS. | 07/09/2026 | 07/09/2026 | [Amazon S3 overview and storage classes](https://000057.awsfcaj.com/1-introduce/)<br>[EBS and instance-store storage on EC2](https://000004.awsfcaj.com/1-introduce/)<br>[Amazon EFS overview](https://000068.awsfcaj.com/4-efsstorageperformance/) |
| Tuesday | Study buckets, object keys, metadata and Regions. Review how prefixes organize objects in S3. | 08/09/2026 | 08/09/2026 | [Amazon S3 overview and storage classes](https://000057.awsfcaj.com/1-introduce/) |
| Wednesday | Read about Block Public Access, bucket policies and encryption. Distinguish access controls from protection of stored data. | 09/09/2026 | 09/09/2026 | [S3 Block Public Access](https://000069.awsfcaj.com/6-s3pba/)<br>[SSE-S3 encryption](https://000069.awsfcaj.com/4-requiresse/) |
| Thursday | Study presigned URLs and CORS. Analyze the browser receiving a URL from the backend and transferring a file directly to S3. | 10/09/2026 | 10/09/2026 | [Share S3 data with a presigned URL](https://000033.awsfcaj.com/6-demo/)<br>[CORS and S3 best practices](https://000057.awsfcaj.com/12-notes/) |
| Friday | Study Versioning, Lifecycle and cost components. Relate S3 file storage to metadata in the CloudDocs database. | 11/09/2026 | 11/09/2026 | [S3 versioning and version storage costs](https://000057.awsfcaj.com/8-versioning/)<br>[CORS and S3 best practices](https://000057.awsfcaj.com/12-notes/) |

</div>

## Weekly reflection

I understood the distinction between an S3 object and the database record describing it. In CloudDocs, the backend should check upload or download permissions before issuing a time-limited access URL.

## Point to clarify

CORS does not replace authorization. An appropriate CORS configuration does not by itself grant bucket read or write permissions.

## Next learning focus

[Week 6: Studying Amazon RDS and comparing it with Amazon DynamoDB](../1.6-Week6/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Amazon S3 overview and storage classes](https://000057.awsfcaj.com/1-introduce/)
- [EBS and instance-store storage on EC2](https://000004.awsfcaj.com/1-introduce/)
- [Amazon EFS overview](https://000068.awsfcaj.com/4-efsstorageperformance/)
- [S3 Block Public Access](https://000069.awsfcaj.com/6-s3pba/)
- [SSE-S3 encryption](https://000069.awsfcaj.com/4-requiresse/)
- [Share S3 data with a presigned URL](https://000033.awsfcaj.com/6-demo/)
- [CORS and S3 best practices](https://000057.awsfcaj.com/12-notes/)
- [S3 versioning and version storage costs](https://000057.awsfcaj.com/8-versioning/)

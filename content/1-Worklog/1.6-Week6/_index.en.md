---
title: "Week 6: Studying Amazon RDS and comparing it with Amazon DynamoDB"
menuTitle: "Week 6 worklog"
date: 2026-11-11
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

**Period:** 14/09/2026 – 18/09/2026.

After file storage, I study business-data persistence. RDS MySQL is the focus, with DynamoDB used to compare data modeling, query patterns and database selection.

## Weekly objectives

- Understand RDS connectivity, access protection and basic backup concepts.
- Distinguish relational modeling from DynamoDB key-value/document modeling.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Study RDS, DB instances, engines and endpoints. Compare a managed database service with self-managed MySQL. | 14/09/2026 | 14/09/2026 | [Database essentials with Amazon RDS](https://000005.awsfcaj.com/) |
| Tuesday | Review DB subnet groups, security groups and TLS. Analyze prerequisites for backend-to-RDS connectivity. | 15/09/2026 | 15/09/2026 | [Database essentials with Amazon RDS](https://000005.awsfcaj.com/)<br>[Security groups](https://000003.awsfcaj.com/2-firewallinvpc/2.1-securitygroup/) |
| Wednesday | Study automated backups, snapshots, Multi-AZ and read replicas. Distinguish recovery, availability and read scaling. | 16/09/2026 | 16/09/2026 | [Database essentials with Amazon RDS](https://000005.awsfcaj.com/) |
| Thursday | Review DynamoDB tables, items, partition keys, sort keys and indexes. Study access-pattern-driven design. | 17/09/2026 | 17/09/2026 | [NoSQL database essentials with DynamoDB](https://000060.awsfcaj.com/) |
| Friday | Compare the options for CloudDocs users, documents and sharing relationships. Explain retaining MySQL for the current model. | 18/09/2026 | 18/09/2026 | [Database essentials with Amazon RDS](https://000005.awsfcaj.com/)<br>[NoSQL database essentials with DynamoDB](https://000060.awsfcaj.com/) |

</div>

## Weekly reflection

I learned to base database selection on relationships and query requirements. DynamoDB is studied as an alternative. MySQL remains the database in the CloudDocs design.

## Point to clarify

Multi-AZ does not replace backups. Maintaining service through infrastructure failures differs from recovering incorrectly modified or deleted data.

## Next learning focus

[Week 7: Studying AWS CLI, AWS CloudShell and IAM role usage](../1.7-Week7/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Database essentials with Amazon RDS](https://000005.awsfcaj.com/)
- [Security groups](https://000003.awsfcaj.com/2-firewallinvpc/2.1-securitygroup/)
- [NoSQL database essentials with DynamoDB](https://000060.awsfcaj.com/)

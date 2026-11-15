---
title: "Week 10: Studying AWS Lambda and resource management with AWS Systems Manager"
menuTitle: "Week 10 worklog"
date: 2026-11-11
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

**Period:** 12/10/2026 – 16/10/2026.

This week covers two complementary areas: event-driven execution with Lambda and server management with Systems Manager. They are studied separately and do not constitute evidence of integration into CloudDocs.

## Weekly objectives

- Understand Lambda functions, triggers, execution roles and execution constraints.
- Understand prerequisites for Session Manager, Run Command and configuration management.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Study Lambda functions, runtimes and triggers. Compare event-driven tasks with a continuously running backend on EC2. | 12/10/2026 | 12/10/2026 | [Serverless automation with AWS Lambda](https://000022.awsfcaj.com/) |
| Tuesday | Review execution roles, timeout, memory and logging. Consider an S3 event-processing task as a possible extension. | 13/10/2026 | 13/10/2026 | [Serverless automation with AWS Lambda](https://000022.awsfcaj.com/) |
| Wednesday | Study Systems Manager and managed nodes. Review SSM Agent, IAM role and service-endpoint connectivity requirements. | 14/10/2026 | 14/10/2026 | [Systems management with Systems Manager](https://000031.awsfcaj.com/) |
| Thursday | Compare Session Manager with SSH and study Run Command. Identify access controls and the scope of affected servers. | 15/10/2026 | 15/10/2026 | [Remote access with Session Manager](https://000058.awsfcaj.com/)<br>[Systems management with Systems Manager](https://000031.awsfcaj.com/) |
| Friday | Review Parameter Store, distinguishing ordinary configuration from sensitive values. Summarize possible CloudDocs operational uses. | 16/10/2026 | 16/10/2026 | [Systems management with Systems Manager](https://000031.awsfcaj.com/) |

</div>

## Weekly reflection

I distinguished Lambda as an event-driven execution environment from Systems Manager as an operations and resource-management service. CloudDocs retains its EC2 backend design. Lambda ideas remain potential extensions.

## Point to clarify

Not every backend function is suitable for Lambda. Session Manager also depends on the server, permissions and service connectivity meeting its prerequisites.

## Next learning focus

[Week 11: Studying Elastic Load Balancing, EC2 Auto Scaling and multi-AZ application deployment](../1.11-Week11/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Serverless automation with AWS Lambda](https://000022.awsfcaj.com/)
- [Systems management with Systems Manager](https://000031.awsfcaj.com/)
- [Remote access with Session Manager](https://000058.awsfcaj.com/)

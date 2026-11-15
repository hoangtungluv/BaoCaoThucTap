---
title: "Week 9: Studying Amazon CloudWatch and system monitoring"
menuTitle: "Week 9 worklog"
date: 2026-11-11
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

**Period:** 05/10/2026 – 09/10/2026.

After studying application components, I consider how to recognize normal operation. CloudWatch is examined through metrics, logs, alarms and correlating failure signals.

## Weekly objectives

- Distinguish metrics, logs, dashboards and alarms.
- Identify monitoring information relevant to EC2, RDS and the CloudDocs backend.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Study metrics, namespaces and dimensions. Review EC2 CPU and RDS database-connection examples. | 05/10/2026 | 05/10/2026 | [Monitoring with Amazon CloudWatch](https://000008.awsfcaj.com/) |
| Tuesday | Review CloudWatch Logs, log groups, streams and retention. Identify application logs worth collecting. | 06/10/2026 | 06/10/2026 | [CloudWatch advanced workshop](https://000036.awsfcaj.com/) |
| Wednesday | Study the CloudWatch Agent. Distinguish default EC2 metrics from operating-system metrics such as memory that require additional collection. | 07/10/2026 | 07/10/2026 | [CloudWatch advanced workshop](https://000036.awsfcaj.com/) |
| Thursday | Review alarm thresholds, evaluation periods and missing-data handling. Study notifications through Amazon SNS. | 08/10/2026 | 08/10/2026 | [Monitoring with Amazon CloudWatch](https://000008.awsfcaj.com/) |
| Friday | Outline a slow-backend investigation: correlate error timing, CPU, database connections and application logs. | 09/10/2026 | 09/10/2026 | [Monitoring with Amazon CloudWatch](https://000008.awsfcaj.com/)<br>[CloudWatch advanced workshop](https://000036.awsfcaj.com/) |

</div>

## Weekly reflection

I learned that one metric rarely establishes the cause of a failure. Metrics should be correlated with logs over the same time window, with thresholds chosen for the application.

## Point to clarify

Passwords, access tokens and presigned URLs should not be logged. Log retention and collection levels also affect monitoring costs.

## Next learning focus

[Week 10: Studying AWS Lambda and resource management with AWS Systems Manager](../1.10-Week10/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Monitoring with Amazon CloudWatch](https://000008.awsfcaj.com/)
- [CloudWatch advanced workshop](https://000036.awsfcaj.com/)

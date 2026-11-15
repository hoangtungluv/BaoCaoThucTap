---
title: "Week 11: Studying Elastic Load Balancing, EC2 Auto Scaling and multi-AZ application deployment"
menuTitle: "Week 11 worklog"
date: 2026-11-11
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

**Period:** 19/10/2026 – 23/10/2026.

This week expands from one server to multiple serving components. I study traffic distribution, instance-count adjustment and reducing dependence on one deployment location.

## Weekly objectives

- Distinguish load balancing, scaling and availability.
- Analyze prerequisites for running the CloudDocs backend across multiple servers.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Compare vertical and horizontal scaling. Identify limitations of increasing the size of a single EC2 instance. | 19/10/2026 | 19/10/2026 | [Scaling applications with EC2 Auto Scaling](https://000006.awsfcaj.com/) |
| Tuesday | Study Application Load Balancers, listeners, target groups and health checks. Trace an HTTP request path. | 20/10/2026 | 20/10/2026 | [Building highly available web applications](https://000101.awsfcaj.com/)<br>[Scaling applications with EC2 Auto Scaling](https://000006.awsfcaj.com/) |
| Wednesday | Review launch templates, Auto Scaling groups and minimum, desired and maximum capacities. Study metric-based scaling policies. | 21/10/2026 | 21/10/2026 | [Scaling applications with EC2 Auto Scaling](https://000006.awsfcaj.com/) |
| Thursday | Study placement across Availability Zones. Distinguish application-tier availability from database-tier availability. | 22/10/2026 | 22/10/2026 | [Building highly available web applications](https://000101.awsfcaj.com/)<br>[Database essentials with Amazon RDS](https://000005.awsfcaj.com/) |
| Friday | Sketch a possible CloudDocs scaling design. Review sessions, local files, shared configuration and database connections across backends. | 23/10/2026 | 23/10/2026 | [Building highly available web applications](https://000101.awsfcaj.com/) |

</div>

## Weekly reflection

I learned that adding servers alone does not establish high availability. Health checks, shared data and remaining failure points must also be considered. The multi-AZ architecture here is an analysis, not a confirmed deployment outcome.

## Point to clarify

Auto Scaling does not resolve every performance bottleneck. Adding backends may not help when database capacity or state management is the limiting factor.

## Next learning focus

[Week 12: Consolidating knowledge, relating it to CloudDocs and completing the internship report](../1.12-Week12/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Scaling applications with EC2 Auto Scaling](https://000006.awsfcaj.com/)
- [Building highly available web applications](https://000101.awsfcaj.com/)
- [Database essentials with Amazon RDS](https://000005.awsfcaj.com/)

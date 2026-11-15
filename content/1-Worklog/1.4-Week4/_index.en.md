---
title: "Week 4: Studying Amazon EC2 and comparing it with Amazon Lightsail"
menuTitle: "Week 4 worklog"
date: 2026-11-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

**Period:** 31/08/2026 – 04/09/2026.

Building on networking concepts, I study server options for running applications. EC2 is the main topic, with Lightsail used to compare resource organization and management complexity.

## Weekly objectives

- Understand AMIs, instance types, EBS and EC2 connection options.
- Compare EC2 and Lightsail in configuration flexibility, operations and cost structure.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Study EC2 instances, AMIs and instance types. Distinguish an operating-system image from compute and memory specifications. | 31/08/2026 | 31/08/2026 | [Amazon EC2 overview](https://000004.awsfcaj.com/1-introduce/) |
| Tuesday | Read about EBS, root volumes and snapshots. Distinguish storage data lifecycles from instance lifecycles. | 01/09/2026 | 01/09/2026 | [Creating and managing EBS snapshots](https://000004.awsfcaj.com/5-amazonec2basic/5.2-createec2snapshot/) |
| Wednesday | Study prerequisites for SSH or Session Manager access to EC2. Review permissions, networking and software requirements. | 02/09/2026 | 02/09/2026 | [Connecting to an Amazon Linux instance](https://000004.awsfcaj.com/4-launchlinuxinstance/4.2-connectlinuxinstance/)<br>[Remote access with Session Manager](https://000058.awsfcaj.com/) |
| Thursday | Review Lightsail and its resource bundles. Compare them with selecting individual components around EC2. | 03/09/2026 | 03/09/2026 | [Getting started with Amazon Lightsail](https://000045.awsfcaj.com/) |
| Friday | Analyze CloudDocs backend hosting needs. Explain why EC2 fits requirements for network configuration, IAM roles and service integration. | 04/09/2026 | 04/09/2026 | [Introduction to Amazon EC2](https://000004.awsfcaj.com/)<br>[IAM roles for EC2](https://000048.awsfcaj.com/) |

</div>

## Weekly reflection

I distinguished server specifications, storage and networking as separate considerations. Choosing EC2 or Lightsail depends on application requirements and operational needs, rather than bundle pricing alone.

## Point to clarify

Stopping an EC2 instance does not end every associated charge. Retained resources such as EBS volumes, snapshots and public IP addresses need separate consideration.

## Next learning focus

[Week 5: Studying Amazon S3 and AWS storage options](../1.5-Week5/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Amazon EC2 overview](https://000004.awsfcaj.com/1-introduce/)
- [Creating and managing EBS snapshots](https://000004.awsfcaj.com/5-amazonec2basic/5.2-createec2snapshot/)
- [Connecting to an Amazon Linux instance](https://000004.awsfcaj.com/4-launchlinuxinstance/4.2-connectlinuxinstance/)
- [Remote access with Session Manager](https://000058.awsfcaj.com/)
- [Getting started with Amazon Lightsail](https://000045.awsfcaj.com/)
- [Introduction to Amazon EC2](https://000004.awsfcaj.com/)
- [IAM roles for EC2](https://000048.awsfcaj.com/)

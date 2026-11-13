---
title: "Week 3: Studying Amazon VPC and networking components"
menuTitle: "Week 3 worklog"
date: 2026-11-11
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

**Period:** 24/08/2026–28/08/2026.

This week examines traffic paths in AWS, from address spaces to access controls. The aim is to interpret a basic network diagram for an application with a server and a database.

## Weekly objectives

- Understand the relationship between VPCs, CIDR blocks, subnets and Availability Zones.
- Distinguish routing from access control using security groups and network ACLs.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Study VPCs and CIDR blocks. Review examples of dividing an address space into non-overlapping subnets. | 24/08/2026 | 24/08/2026 | [Amazon VPC and networking](https://000003.awsfcaj.com/1-introduce/)<br>[VPC subnets](https://000003.awsfcaj.com/1-introduce/1.1-subnets/) |
| Tuesday | Distinguish public and private subnets through routing configuration. Study how subnets relate to Availability Zones. | 25/08/2026 | 25/08/2026 | [VPC subnets](https://000003.awsfcaj.com/1-introduce/1.1-subnets/) |
| Wednesday | Study route tables, internet gateways and NAT gateways. Analyze outbound Internet paths for different resources. | 26/08/2026 | 26/08/2026 | [Route tables](https://000003.awsfcaj.com/1-introduce/1.2-routetable/)<br>[NAT gateways](https://000003.awsfcaj.com/1-introduce/1.4-natgateway/) |
| Thursday | Compare security groups and network ACLs in scope, connection state and rule processing. | 27/08/2026 | 27/08/2026 | [Security groups](https://000003.awsfcaj.com/2-firewallinvpc/2.1-securitygroup/)<br>[Network ACLs](https://000003.awsfcaj.com/2-firewallinvpc/2.2-networkacls/) |
| Friday | Review a server-and-database network diagram. Identify required connections and paths that should be restricted. | 28/08/2026 | 28/08/2026 | [Amazon VPC and networking](https://000003.awsfcaj.com/1-introduce/)<br>[Database essentials with Amazon RDS](https://000005.awsfcaj.com/) |

</div>

## Weekly reflection

I learned that connectivity depends on several layers: addressing, routing, network access controls and service configuration. A network diagram helps investigate each layer rather than changing multiple settings at once.

## Point to clarify

Placing a resource in a public subnet does not by itself ensure Internet reachability. Public addressing, routes and access rules must also be considered.

## Next learning focus

[Week 4: Studying Amazon EC2 and comparing it with Amazon Lightsail](../1.4-Week4/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Amazon VPC and networking](https://000003.awsfcaj.com/1-introduce/)
- [VPC subnets](https://000003.awsfcaj.com/1-introduce/1.1-subnets/)
- [Route tables](https://000003.awsfcaj.com/1-introduce/1.2-routetable/)
- [NAT gateways](https://000003.awsfcaj.com/1-introduce/1.4-natgateway/)
- [Security groups](https://000003.awsfcaj.com/2-firewallinvpc/2.1-securitygroup/)
- [Network ACLs](https://000003.awsfcaj.com/2-firewallinvpc/2.2-networkacls/)
- [Database essentials with Amazon RDS](https://000005.awsfcaj.com/)

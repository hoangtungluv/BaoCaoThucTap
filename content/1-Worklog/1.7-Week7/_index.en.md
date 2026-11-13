---
title: "Week 7: Studying AWS CLI, AWS CloudShell and IAM role usage"
menuTitle: "Week 7 worklog"
date: 2026-11-11
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

**Period:** 21/09/2026–25/09/2026.

This week moves from recognizing services to interacting with resources through command-line tools. I revisit IAM roles in the context of credentials and service access from a working environment or EC2.

## Weekly objectives

- Understand AWS CLI, profiles, Regions and the AWS CloudShell environment.
- Distinguish long-term credentials from temporary role credentials.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Review AWS CLI command structure and help. Study the effects of Region selection and output formats. | 21/09/2026 | 21/09/2026 | [Getting started with AWS CLI](https://000011.awsfcaj.com/) |
| Tuesday | Study profiles and credential sources. Analyze aws sts get-caller-identity as a way to identify the current principal. | 22/09/2026 | 22/09/2026 | [Getting started with AWS CLI](https://000011.awsfcaj.com/)<br>[AWS CLI with IAM](https://000011.awsfcaj.com/7-iam/) |
| Wednesday | Study AWS CloudShell, its browser-based command environment and permissions associated with the signed-in session. | 23/09/2026 | 23/09/2026 | [Installing AWS CLI](https://000011.awsfcaj.com/3-installcli/)<br>[Getting started with AWS CLI](https://000011.awsfcaj.com/) |
| Thursday | Review IAM roles for EC2 and instance profiles. Compare temporary credential retrieval with embedding access keys in source code. | 24/09/2026 | 24/09/2026 | [IAM roles for EC2](https://000048.awsfcaj.com/) |
| Friday | Analyze resource-inspection commands and error scenarios. Summarize checking identity, Region and permissions before changing configuration. | 25/09/2026 | 25/09/2026 | [AWS CLI troubleshooting](https://000011.awsfcaj.com/10-troubleshoot/)<br>[AWS CLI with IAM](https://000011.awsfcaj.com/7-iam/) |

</div>

## Weekly reflection

I learned that the same command can behave differently with a different principal, Region or account. Week 2 IAM concepts are connected to the case of an application on EC2 accessing S3.

## Point to clarify

CloudShell provides a command environment, not a way around IAM restrictions. Before a modifying command, identify the target account and Region.

## Next learning focus

[Week 8: Studying Amazon Cognito, user authentication and token-based access control](../1.8-Week8/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Getting started with AWS CLI](https://000011.awsfcaj.com/)
- [AWS CLI with IAM](https://000011.awsfcaj.com/7-iam/)
- [Installing AWS CLI](https://000011.awsfcaj.com/3-installcli/)
- [IAM roles for EC2](https://000048.awsfcaj.com/)
- [AWS CLI troubleshooting](https://000011.awsfcaj.com/10-troubleshoot/)

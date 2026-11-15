---
title: "Week 2: Studying AWS IAM and access management"
menuTitle: "Week 2 worklog"
date: 2026-11-11
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

**Period:** 17/08/2026 – 21/08/2026.

After reviewing AWS accounts, I focus on who can perform which actions on resources. This week covers IAM components and interpreting access permissions.

## Weekly objectives

- Distinguish IAM users, groups, policies and roles.
- Understand least privilege and an approach to investigating AccessDenied errors.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Study IAM users and groups. Distinguish an identity from a group used to organize permissions. | 17/08/2026 | 17/08/2026 | [IAM groups and users](https://000002.awsfcaj.com/1-introduction/1.1-group-user/) |
| Tuesday | Read IAM policy structure, focusing on Effect, Action, Resource and Condition. Analyze permission examples. | 18/08/2026 | 18/08/2026 | [IAM policies](https://000002.awsfcaj.com/1-introduction/1.2-iam-policy/) |
| Wednesday | Study IAM roles, trust policies and temporary credentials. Distinguish role permissions from who can assume a role. | 19/08/2026 | 19/08/2026 | [IAM roles](https://000002.awsfcaj.com/1-introduction/1.3-iam-role/) |
| Thursday | Review permission evaluation and explicit deny. Compare examples of allowed and denied access. | 20/08/2026 | 20/08/2026 | [IAM policies](https://000002.awsfcaj.com/1-introduction/1.2-iam-policy/)<br>[Access management with IAM](https://000002.awsfcaj.com/) |
| Friday | Summarize an AccessDenied investigation: identify the principal, action, resource and relevant policies. | 21/08/2026 | 21/08/2026 | [Switching IAM roles](https://000002.awsfcaj.com/4-switch-roles/)<br>[IAM policies](https://000002.awsfcaj.com/1-introduction/1.2-iam-policy/) |

</div>

## Weekly reflection

I distinguished organizing users from granting permissions. An IAM configuration should be considered in terms of both allowed actions and the conditions under which an identity can use those permissions.

## Point to clarify

An access failure should not immediately lead to granting AdministratorAccess. Identify the missing action or denial condition before proposing a permission change.

## Next learning focus

[Week 3: Studying Amazon VPC and networking components](../1.3-Week3/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [IAM groups and users](https://000002.awsfcaj.com/1-introduction/1.1-group-user/)
- [IAM policies](https://000002.awsfcaj.com/1-introduction/1.2-iam-policy/)
- [IAM roles](https://000002.awsfcaj.com/1-introduction/1.3-iam-role/)
- [Access management with IAM](https://000002.awsfcaj.com/)
- [Switching IAM roles](https://000002.awsfcaj.com/4-switch-roles/)

---
title: "Week 8: Studying Amazon Cognito, user authentication and token-based access control"
menuTitle: "Week 8 worklog"
date: 2026-11-11
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

**Period:** 28/09/2026 – 02/10/2026.

This week focuses on application-user identity. I distinguish Cognito sign-in from document permissions enforced by the CloudDocs backend.

## Weekly objectives

- Understand user pools, app clients and how to integrate Cognito into a web application.
- Distinguish ID, access and refresh tokens from business-level authorization.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Study User Pools, app clients and user states. Distinguish application users from IAM users. | 28/09/2026 | 28/09/2026 | [Create a Cognito user pool and app client](https://000081.awsfcaj.com/2-create-user-pool/) |
| Tuesday | Study how to integrate a Cognito user pool into a web application. Review the User Pool ID, app client ID and Region settings in the application. | 29/09/2026 | 29/09/2026 | [Integrate Cognito into a SPA](https://000055.awsfcaj.com/4-configure-aaa/4.1-add-authentication-with-cognito/) |
| Wednesday | Compare ID, access and refresh tokens in purpose, lifetime and session renewal. | 30/09/2026 | 30/09/2026 | [Distinguish Cognito sign-in tokens](https://000081.awsfcaj.com/3-create-api-and-lambda-function/) |
| Thursday | Study Cognito authorizers in API Gateway. Review how to read tokens from the Authorization header and use claims to identify the user calling an API. | 01/10/2026 | 01/10/2026 | [Protect an API with a Cognito authorizer](https://000117.awsfcaj.com/6-identity/6.8-authorizer/) |
| Friday | Relate missing or expired tokens and insufficient document permissions to authentication versus authorization failures. | 02/10/2026 | 02/10/2026 | [API authentication and unauthorized responses](https://000055.awsfcaj.com/4-configure-aaa/4.2-setup-authentication/)<br>[Cognito sign-in and token types](https://000081.awsfcaj.com/3-create-api-and-lambda-function/) |

</div>

## Weekly reflection

I distinguished identifying a user from deciding which documents the user may access. A valid token is an input condition. The backend must still enforce ownership, sharing and account-status rules.

## Point to clarify

Decoding a JWT does not establish trust. Its signature and appropriate claims must be validated. Signing out should not be assumed to invalidate every issued token immediately in every verifier.

## Next learning focus

[Week 9: Studying Amazon CloudWatch and system monitoring](../1.9-Week9/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Create a Cognito user pool and app client](https://000081.awsfcaj.com/2-create-user-pool/)
- [Integrate Cognito into a SPA](https://000055.awsfcaj.com/4-configure-aaa/4.1-add-authentication-with-cognito/)
- [Distinguish Cognito sign-in tokens](https://000081.awsfcaj.com/3-create-api-and-lambda-function/)
- [Protect an API with a Cognito authorizer](https://000117.awsfcaj.com/6-identity/6.8-authorizer/)
- [API authentication and unauthorized responses](https://000055.awsfcaj.com/4-configure-aaa/4.2-setup-authentication/)

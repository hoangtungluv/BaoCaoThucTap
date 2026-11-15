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

- Understand User Pools, app clients and the Authorization Code flow with PKCE.
- Distinguish ID, access and refresh tokens from business-level authorization.

## Learning activities

<div class="worklog-table" tabindex="0" role="region" aria-label="Weekly worklog. Scroll horizontally to view all columns.">

| Day | Study and review activity | Start date | Completion date | Study sources |
| --- | --- | --- | --- | --- |
| Monday | Study User Pools, app clients and user states. Distinguish application users from IAM users. | 28/09/2026 | 28/09/2026 | [Cross-site authentication with Cognito](https://000141.awsfcaj.com/) |
| Tuesday | Review sign-in pages, callback and logout URLs. Analyze the Authorization Code flow with PKCE for web applications. | 29/09/2026 | 29/09/2026 | [Deploying and testing Cognito](https://000141.awsfcaj.com/4-app-configuration/) |
| Wednesday | Compare ID, access and refresh tokens in purpose, lifetime and session renewal. | 30/09/2026 | 30/09/2026 | [Cognito integration code explanation](https://000141.awsfcaj.com/3-note-code/) |
| Thursday | Study JWT signature, issuer, expiry, token_use and application-identifier checks appropriate to each token type. | 01/10/2026 | 01/10/2026 | [Cognito integration code explanation](https://000141.awsfcaj.com/3-note-code/) |
| Friday | Relate missing or expired tokens and insufficient document permissions to authentication versus authorization failures. | 02/10/2026 | 02/10/2026 | [Deploying and testing Cognito](https://000141.awsfcaj.com/4-app-configuration/)<br>[Cognito integration code explanation](https://000141.awsfcaj.com/3-note-code/) |

</div>

## Weekly reflection

I distinguished identifying a user from deciding which documents the user may access. A valid token is an input condition. The backend must still enforce ownership, sharing and account-status rules.

## Point to clarify

Decoding a JWT does not establish trust. Its signature and appropriate claims must be validated. Signing out should not be assumed to invalidate every issued token immediately in every verifier.

## Next learning focus

[Week 9: Studying Amazon CloudWatch and system monitoring](../1.9-Week9/).

## References

- [Cloud Journey — Learning catalogue](https://cloudjourney.awsfcaj.com/)
- [Cross-site authentication with Cognito](https://000141.awsfcaj.com/)
- [Deploying and testing Cognito](https://000141.awsfcaj.com/4-app-configuration/)
- [Cognito integration code explanation](https://000141.awsfcaj.com/3-note-code/)

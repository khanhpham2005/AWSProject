---
title: "Week 8 Worklog"
date: 2026-07-20
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 objectives

* Integrate Amazon Cognito for user authentication management.
* Isolate data by user, ensuring privacy for each account.

### Tasks during the week (20/07 - 24/07/2026)

| Day | Task | Start | End | Reference |
| --- | --- | --- | --- | --- |
| Mon | Initialize Cognito User Pool and App Client (`USER_PASSWORD_AUTH` mode), saving Pool ID and Client ID configurations. | 20/07/2026 | 20/07/2026 | [Cognito lab](https://000081.awsstudygroup.com) |
| Tue | Integrate JWT Authorizer into API Gateway and open public OPTIONS routes to handle CORS preflight. | 21/07/2026 | 21/07/2026 |  |
| Wed | Update Lambda to extract `sub` claims from JWTs to identify users and filter data accordingly. | 22/07/2026 | 22/07/2026 |  |
| Thu | Connect registration, confirmation, and login flows directly from the frontend using `cognito-idp` without external libraries. | 23/07/2026 | 23/07/2026 |  |
| Fri | Test the entire flow: register → confirm → log in → invoke API with token (200), without token (401), and OPTIONS (200). | 24/07/2026 | 24/07/2026 | Postman |

### Results achieved

1. Completed user authentication system via Cognito; secured API Gateway using a JWT Authorizer.
2. Ensured user data privacy: Lambda automatically enforces permissions and returns only files owned by the respective user.
3. Fully handled CORS preflight flows via OPTIONS routes, ensuring the API correctly blocks unauthorized requests.

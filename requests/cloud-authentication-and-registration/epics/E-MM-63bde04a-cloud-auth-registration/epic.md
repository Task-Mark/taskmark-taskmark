---
id: E-MM-63bde04a
type: epic
title: Cloud authentication and registration
status: backlog
priority: high
size: null
points: null
parent: null
epic: null
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, api, auth]
created: 2026-09-02
updated: 2026-09-02T15:28:10Z
started_at: null
completed_at: null
---
# E-MM-63bde04a: Cloud authentication and registration

## Description

Stand up first-party authentication for Taskmark Cloud: NestJS accounts on MongoDB, a pending project created at signup, email verification, and project invitations sent with Resend. The hosted board itself stays out of scope.

```mermaid
flowchart TD
  register["Register: account + project + emails"] --> pending[User and project pending]
  pending --> verifyMail[Verification email via Resend]
  verifyMail --> verify[Confirm email]
  verify --> activate[Activate account, project, and owner]
  activate --> inviteMail[Send invitations]
  inviteMail --> existing[Existing user logs in and accepts]
  inviteMail --> newUser[New user creates and verifies an account]
  existing --> member[Active member]
  newUser --> member
  login[Login] --> access[Short-lived access cookie]
  access --> refresh[Rotating HttpOnly refresh cookie]
```

## Goal

A person can register, verify email, sign in with secure cookies, name a first project, and invite others by email without exposing credentials or enumerating accounts.

## Acceptance criteria

- [ ] Registration creates a pending user and pending project and does not start a session.
- [ ] Email verification activates the owner membership and then sends invitations.
- [ ] Login issues rotating HttpOnly access and refresh cookies.
- [ ] Invitations work for both existing and unknown emails.
- [ ] Secrets stay in local env files; no live credentials are committed.

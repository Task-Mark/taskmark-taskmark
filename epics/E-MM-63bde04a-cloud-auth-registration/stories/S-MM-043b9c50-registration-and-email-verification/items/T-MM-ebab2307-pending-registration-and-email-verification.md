---
id: T-MM-ebab2307
type: task
title: Implement pending registration and email verification
status: done
priority: high
size: L
points: 8
parent: S-MM-043b9c50
epic: E-MM-63bde04a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [auth]
created: 2026-09-02
updated: 2026-09-02T16:23:30Z
started_at: 2026-09-02T15:28:10Z
completed_at: 2026-09-02T15:52:15Z
---
# T-MM-ebab2307: Implement pending registration and email verification

## Description

Add register, verify-email, and resend-verification endpoints that keep the account and first project pending until the hashed one-time email token is confirmed.

## Acceptance criteria

- [x] `POST /v1/auth/register` creates a pending user, project, and owner membership and returns 202 without cookies.
- [x] Passwords use Argon2id; verification tokens are stored hashed; responses do not enumerate emails.
- [x] Verifying email activates the user, project, and owner membership.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | From the Cloud Auth Registration plan: implement pending registration, owner project, and email verification. |
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T16:23:30Z | prompt | Marco Mendão | Passwords must be at least 8 characters, not 10. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T15:28:10Z | 2026-09-02T15:52:15Z | Added pending register, hashed verification, and activation of the owner project. |
| Marco Mendão | 2026-09-02T16:23:00Z | 2026-09-02T16:23:30Z | Lowered the minimum password length from 10 to 8. |

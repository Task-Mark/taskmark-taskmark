---
id: T-MM-85724aaf
type: task
title: Send and accept project invitations with Resend
status: done
priority: high
size: L
points: 8
parent: S-MM-9f272fd9
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
tags: [invites, resend]
created: 2026-09-02
updated: 2026-09-02T15:52:15Z
started_at: 2026-09-02T15:28:10Z
completed_at: 2026-09-02T15:52:15Z
---
# T-MM-85724aaf: Send and accept project invitations with Resend

## Description

Create hashed project invitations after the owner verifies email, send them with Resend, and let existing or new users accept from a token link.

## Acceptance criteria

- [x] One pending invitation exists per project and email.
- [x] Existing users accept after login; new users register from the invite, verify, and join.
- [x] Mail is sent through a testable Resend wrapper using env-only credentials.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | From the Cloud Auth Registration plan: implement invitations for existing and new users and deliver them with Resend. |
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T15:28:10Z | 2026-09-02T15:52:15Z | Created hashed invitations after owner verify, Resend delivery, accept, and register-from-invite. |

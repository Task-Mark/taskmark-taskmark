---
id: T-MM-27707b69
type: task
title: Build cloud login and registration wizard
status: done
priority: high
size: L
points: 8
parent: S-MM-4ba20e58
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
tags: [cloud, ui]
created: 2026-09-02
updated: 2026-09-02T16:20:10Z
started_at: 2026-09-02T15:28:10Z
completed_at: 2026-09-02T15:52:15Z
---
# T-MM-27707b69: Build cloud login and registration wizard

## Description

Add Taskmark-styled login, a four-step registration wizard, email verification, and invite acceptance in `taskmark-cloud`, talking to the API through a same-origin cookie-preserving proxy.

## Acceptance criteria

- [x] Public pages exist for login, register, verify-email, and invite tokens.
- [x] Registration walks Account, Project, Invites, then Verify email.
- [x] Unauthenticated visitors cannot stay on the board; authenticated users skip login.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | From the Cloud Auth Registration plan: create login, the registration wizard, verification, and invite acceptance in taskmark-cloud. |
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T16:20:10Z | prompt | Marco Mendão | Registration must include password and retype password, validated with React Hook Form. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T15:28:10Z | 2026-09-02T15:52:15Z | Built login, the four-step wizard, verify and invite pages, plus a cookie-preserving API proxy. |
| Marco Mendão | 2026-09-02T16:17:00Z | 2026-09-02T16:20:10Z | Added password and retype password fields with React Hook Form on registration. |

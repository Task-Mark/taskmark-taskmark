---
id: T-MM-8f09153a
type: task
title: Issue rotating HttpOnly access and refresh cookies
status: done
priority: high
size: M
points: 5
parent: S-MM-5a28bda4
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
tags: [auth, cookies]
created: 2026-09-02
updated: 2026-09-02T15:52:15Z
started_at: 2026-09-02T15:28:10Z
completed_at: 2026-09-02T15:52:15Z
---
# T-MM-8f09153a: Issue rotating HttpOnly access and refresh cookies

## Description

Add login, refresh, logout, and me for active users, storing short-lived access and rotating refresh tokens in HttpOnly cookies.

## Acceptance criteria

- [x] Only verified active users can log in.
- [x] Access and refresh cookies are HttpOnly with SameSite=Lax and Secure in production.
- [x] Refresh rotation revokes a family when a used token is presented again.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | From the Cloud Auth Registration plan: implement login, access/refresh cookies, rotation, logout, and a JWT guard. |
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T15:28:10Z | 2026-09-02T15:52:15Z | Issued rotating HttpOnly cookies, family revocation on reuse, logout, and `/me`. |

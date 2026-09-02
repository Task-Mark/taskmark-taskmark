---
id: T-MM-698aaabb
type: task
title: Cover auth flows with unit and e2e tests
status: done
priority: high
size: M
points: 5
parent: E-MM-63bde04a
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
tags: [tests, security]
created: 2026-09-02
updated: 2026-09-02T15:52:15Z
started_at: 2026-09-02T15:28:10Z
completed_at: 2026-09-02T15:52:15Z
---
# T-MM-698aaabb: Cover auth flows with unit and e2e tests

## Description

Add unit tests for hashing, token rotation, and email normalization, plus e2e coverage of register-verify-login-refresh and invitations, then lint and build the API and cloud app.

## Acceptance criteria

- [x] Unit tests cover hashing, refresh reuse revocation, and invite email normalization.
- [x] E2e covers register, verify, login, refresh, logout, and invite accept for existing and new users.
- [x] API and cloud lint/build succeed and no secrets appear in tracked files.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | From the Cloud Auth Registration plan: cover the flows with unit and e2e tests and validate builds. |
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T15:28:10Z | 2026-09-02T15:52:15Z | Added unit and e2e coverage, fixed Nest e2e bootstrap against MongoMemoryServer, and confirmed lint/build. |

---
id: S-MM-0dda88f5
type: story
title: Secure API foundation
status: backlog
priority: high
size: null
points: null
parent: E-MM-63bde04a
epic: E-MM-63bde04a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [api, mongodb]
created: 2026-09-02
updated: 2026-09-02T15:28:10Z
started_at: null
completed_at: null
---
# S-MM-0dda88f5: Secure API foundation

## User story

As a cloud operator, I want the NestJS API configured with validated env, MongoDB models, and baseline HTTP hardening, so later auth features sit on a safe substrate.

## Acceptance criteria

- [ ] The API starts only when required env is present and valid.
- [ ] User, project, membership, invitation, verification, and refresh-session models exist with unique indexes.
- [ ] HTTP uses `/v1`, validation, Helmet, CORS, and rate limiting.

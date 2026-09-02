---
id: S-MM-5a28bda4
type: story
title: Login and session cookies
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
tags: [auth, session]
created: 2026-09-02
updated: 2026-09-02T15:28:10Z
started_at: null
completed_at: null
---
# S-MM-5a28bda4: Login and session cookies

## User story

As a verified user, I want to sign in with cookies that rotate safely, so I can use the cloud app without storing tokens in the browser.

## Acceptance criteria

- [ ] Login, refresh, logout, and me endpoints exist for active users only.
- [ ] Access and refresh tokens live in HttpOnly cookies with SameSite=Lax.
- [ ] Refresh tokens rotate by family and reuse revokes that family.

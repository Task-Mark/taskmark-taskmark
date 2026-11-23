---
id: S-MM-043b9c50
type: story
title: Registration and email verification
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
tags: [auth, email]
created: 2026-09-02
updated: 2026-09-02T15:28:10Z
started_at: null
completed_at: null
---
# S-MM-043b9c50: Registration and email verification

## User story

As a new Taskmark Cloud user, I want to create an account and a first project that stay pending until I confirm my email, so unused addresses cannot immediately join a workspace.

## Acceptance criteria

- [ ] Register accepts name, email, password, project name, and invite emails and returns 202 without a session.
- [ ] Passwords are hashed with Argon2id; only hashed verification tokens are stored.
- [ ] Confirming email activates the user, project, and owner membership.

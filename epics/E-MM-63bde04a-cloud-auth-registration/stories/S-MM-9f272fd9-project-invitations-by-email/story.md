---
id: S-MM-9f272fd9
type: story
title: Project invitations by email
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
tags: [invites, resend]
created: 2026-09-02
updated: 2026-09-02T15:28:10Z
started_at: null
completed_at: null
---
# S-MM-9f272fd9: Project invitations by email

## User story

As a project owner, I want to invite people by email whether or not they already have an account, so they can join after they authenticate as that address.

## Acceptance criteria

- [ ] One pending invitation exists per project and email, with a hashed one-time token.
- [ ] Existing users log in and accept; new users register, verify, and then join.
- [ ] Resend delivers invite and verification mail using env configuration only.

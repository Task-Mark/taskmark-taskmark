---
id: S-MM-54ca5d61
type: story
title: Project sync token
status: backlog
priority: high
size: null
points: null
parent: E-MM-495d489d
epic: E-MM-495d489d
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, auth, sync]
created: 2026-09-02
updated: 2026-09-02T17:54:46Z
started_at: null
completed_at: null
---
# S-MM-54ca5d61: Project sync token

## Description

Give each cloud project one recoverable sync token that local Taskmark instances use as `TASKMARK_SYNC_TOKEN`. The token identifies the project and authorizes board sync without a local project id.

## User story

As a project member, I can copy one sync token from Settings and send it to other developers so their local boards sync to this project automatically.

## Acceptance criteria

- [ ] Each project has exactly one current sync token with a recognizable prefix.
- [ ] Active members can view and copy the token; only the owner can rotate it.
- [ ] Local sync requests authenticate with the bearer token and never send a project id.

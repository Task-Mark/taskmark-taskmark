---
id: S-MM-d8e0226d
type: story
title: Local CLI board sync
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
tags: [cli, sync]
created: 2026-09-02
updated: 2026-09-02T17:54:46Z
started_at: null
completed_at: null
---
# S-MM-d8e0226d: Local CLI board sync

## Description

Let `@taskmark/ui` push the current board using `TASKMARK_SYNC_TOKEN`, optionally watching markdown changes and running alongside local `dev` or `serve`.

## User story

As a developer, I set `TASKMARK_SYNC_TOKEN` on my machine and run `npx taskmark sync --watch` so local markdown edits reach the cloud without configuring a project id.

## Acceptance criteria

- [ ] Sync uses only env vars for token and optional cloud URL; the token selects the project.
- [ ] Watch mode rebuilds the snapshot and sends a hash-diffed file batch after markdown changes.
- [ ] A rotated or invalid token stops sync with a clear unauthorized message.

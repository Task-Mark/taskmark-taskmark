---
id: S-MM-78cafdeb
type: story
title: Store synced board files and snapshot
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
tags: [cloud, api, sync]
created: 2026-09-02
updated: 2026-09-02T17:54:46Z
started_at: null
completed_at: null
---
# S-MM-78cafdeb: Store synced board files and snapshot

## Description

Accept batches of relative markdown files and a BoardSnapshot cache from local clients, keep files as the source of truth, and serve snapshot plus version for the hosted board.

## User story

As a local Taskmark instance, I can push only files whose hashes changed and trust the API to store the merged board and expose a snapshot the cloud UI can render.

## Acceptance criteria

- [ ] Manifest lists stored paths and hashes so clients can diff.
- [ ] A sync batch upserts or deletes allowed board paths and replaces the snapshot cache, incrementing a version.
- [ ] Cookie-authenticated project members can read snapshot and version.

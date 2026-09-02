---
id: S-MM-d06399f8
type: story
title: Hosted read-only board
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
tags: [cloud, ui]
created: 2026-09-02
updated: 2026-09-02T17:54:46Z
started_at: null
completed_at: null
---
# S-MM-d06399f8: Hosted read-only board

## Description

Replace the cloud board stub with the shared board UI fed by the stored snapshot, refresh when the sync version changes, and explain how to start syncing when no snapshot exists.

## User story

As a signed-in project member, I see the same board as local Taskmark, updated after developers sync, without being able to edit items in the cloud.

## Acceptance criteria

- [ ] The cloud board renders from the project snapshot using shared board components.
- [ ] The UI refreshes when the stored board version changes.
- [ ] An empty state points to Settings and the `TASKMARK_SYNC_TOKEN` setup.

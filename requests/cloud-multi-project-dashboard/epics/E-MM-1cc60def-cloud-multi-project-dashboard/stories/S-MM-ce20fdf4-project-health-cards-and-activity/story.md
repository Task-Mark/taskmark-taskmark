---
id: S-MM-ce20fdf4
type: story
title: Project health cards and global activity feed
status: backlog
priority: high
size: null
points: null
parent: E-MM-1cc60def
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, dashboard, projects, activity]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# S-MM-ce20fdf4: Project health cards and global activity feed

## Description

Per-project health at a glance and a merged activity stream: a card per project (progress, velocity, contributors, last sync) linking to its board, a top-of-page banner calling out projects whose sync has gone stale, and a global feed of recent worklog activity across all projects.

## User story

As a Cloud user, I want to see each project's health and a merged stream of recent activity so I can spot stalled projects and follow what just happened everywhere.

## Acceptance criteria

- [ ] Each project renders a card with done/total progress, velocity, contributors, last sync, and a link to its board.
- [ ] Projects without a sync for more than 7 days (or never synced) are flagged on their card and listed in a top banner linking to setup instructions.
- [ ] A merged activity feed shows recent worklog events across projects, newest first, with a project badge per row.

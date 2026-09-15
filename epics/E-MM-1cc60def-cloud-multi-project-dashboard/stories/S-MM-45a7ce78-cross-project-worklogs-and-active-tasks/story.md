---
id: S-MM-45a7ce78
type: story
title: Cross-project worklogs and active tasks tables
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
tags: [cloud, dashboard, worklog, tables]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# S-MM-45a7ce78: Cross-project worklogs and active tasks tables

## Description

Two tables that answer "what has been done" and "what is being done": a paginated global worklog table merging every project's sessions with a project column, and a sortable table of active tasks and bugs across all projects. Rows link to the owning project board (the per-board detail sheet cannot open cross-project).

## User story

As a Cloud user, I want to scan all recent work sessions and every active task across projects in two tables so I can follow the work without opening each board.

## Acceptance criteria

- [ ] The worklog table merges all projects newest-first with actor, item, project, session dates, and summary, paginated.
- [ ] The active tasks table lists `in_progress` and `blocked` items across projects, sortable by priority, project, and last update.
- [ ] Rows link to the owning project board and both tables honour the global filters.

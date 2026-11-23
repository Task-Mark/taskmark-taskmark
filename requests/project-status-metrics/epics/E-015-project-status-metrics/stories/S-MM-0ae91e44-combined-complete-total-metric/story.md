---
id: S-MM-0ae91e44
type: story
title: Combined complete/total work item metric
status: backlog
priority: medium
size: null
points: null
parent: E-015
epic: E-015
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, metrics, dashboard]
created: 2026-08-30
updated: 2026-08-30T06:46:00Z
started_at: null
completed_at: null
---

# S-MM-0ae91e44: Combined complete/total work item metric

## User story

As a project lead looking at Overall, I want a single work-item card that shows complete over total (for example `400/500`) so I can see volume and completion together, and I want those two numbers to match when every countable item is complete.

## Acceptance criteria

- [ ] The Total work items and Complete work items cards are replaced by one metric card titled Complete work items.
- [ ] The large value is `total/complete` in the form `500/400` (total first, then complete).
- [ ] When every countable story, task, and bug is terminal, the two numbers are equal (for example `500/500`).
- [ ] Current week, Current Speed, contributors, and the heatmap stay as they are aside from the tighter metrics row.

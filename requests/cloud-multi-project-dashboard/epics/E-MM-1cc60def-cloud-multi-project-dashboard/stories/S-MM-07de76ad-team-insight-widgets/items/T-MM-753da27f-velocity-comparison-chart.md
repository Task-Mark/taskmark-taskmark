---
id: T-MM-753da27f
type: task
title: Velocity comparison across projects
status: backlog
priority: medium
size: S
points: 3
parent: S-MM-07de76ad
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, velocity]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-753da27f: Velocity comparison across projects

## Description

Side-by-side horizontal bars per project comparing average velocity (`currentSpeedPtsPerWeek`) with peak (`peakSpeedPtsPerWeek`), both already in `statusMetrics`, formatted with `formatSpeedPtsPerWeek` and labelling the peak ISO week (`peakSpeedWeekLabel`). Projects without speed data show a dash instead of an empty bar.

## Acceptance criteria

- [ ] Each selected project shows current vs peak pts/week bars with the peak week label.
- [ ] Values match `formatSpeedPtsPerWeek` formatting used on the boards.
- [ ] Projects with no completions render a clear "no data" state, not zero-height bars.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — average vs peak velocity comparison per project. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

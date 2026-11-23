---
id: T-MM-3322b284
type: task
title: Task vs bug distribution mini-gauge
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
tags: [cloud, frontend, charts]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-3322b284: Task vs bug distribution mini-gauge

## Description

Mini gauge/pie for the filtered period counting completions by `itemType` from the enriched completion samples, reusing the shared chart primitives in `@taskmark/components` (`components/charts`: `Gauge` / `PieCenter`). Shows the proportion of feature work (tasks) versus bug fixing.

## Acceptance criteria

- [ ] The widget shows the task vs bug completion split for the filtered period across selected projects.
- [ ] It reuses the shared `components/charts` primitives rather than a new chart implementation.
- [ ] An empty period renders a neutral empty state.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — task vs bug completion split mini-gauge. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

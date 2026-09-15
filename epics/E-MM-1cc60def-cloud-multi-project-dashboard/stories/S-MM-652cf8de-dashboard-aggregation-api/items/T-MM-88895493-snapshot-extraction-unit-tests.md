---
id: T-MM-88895493
type: task
title: Unit tests for dashboard snapshot extraction
status: backlog
priority: high
size: S
points: 3
parent: S-MM-652cf8de
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [api, tests, dashboard]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-88895493: Unit tests for dashboard snapshot extraction

## Description

Jest specs for the dashboard service extraction helpers, in the style of the existing `board-activity.spec.ts`: flattening worklog rows from `detailsByPath` with the 90-day window and per-project cap, building completion samples with resolvers, selecting active items by status, and tolerating malformed snapshots (missing keys, wrong types, null snapshot).

## Acceptance criteria

- [ ] Specs cover worklog flattening, window and cap behaviour, completion-sample enrichment, and active-item selection.
- [ ] Malformed and empty snapshots produce empty results without throwing.
- [ ] `npm test` in taskmark-api passes with the new specs.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — unit tests for the dashboard snapshot extraction helpers. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

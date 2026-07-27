---
id: T-147
type: task
title: Sort work items by id, title, size, and epic
status: backlog
priority: medium
size: M
size_source: suggested
size_basis: [T-100, T-131]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-049
epic: E-013
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-07-27T05:16:43.229Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-147: Sort work items by id, title, size, and epic

## Description

Wire the Work items table to shared sort for **id**, **title**, **size**, and **epic**.

## Acceptance criteria

- [ ] Work items headers for ID, Title, Size, and Epic are sortable.
- [ ] Epic sort uses a stable key (epic title with id tie-break, or epic id) and places missing-epic rows consistently.
- [ ] Asc/desc reorder the filtered result set correctly.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:19:23Z | prompt | Marco Mendão | Create stories and tasks for E-013 table sort (epic, size, title, id) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

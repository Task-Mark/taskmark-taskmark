---
id: T-157
type: task
title: Document one-command UI launch on board init
status: backlog
priority: medium
size: M
size_source: suggested
size_basis: [T-028, T-156]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-052
epic: E-014
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, init, docs]
created: 2026-07-24
updated: 2026-07-27T05:37:38.663Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-157: Document one-command UI launch on board init

## Description

Update Taskmark init / board README (and related plugin docs) so a newly created board tells the user to run `npx taskmark serve` and open `http://localhost:8275`.

## Acceptance criteria

- [ ] New boards (or init output) include `npx taskmark serve` and port **8275**.
- [ ] Nested and flat board layouts are both covered.
- [ ] Wording does not require cloning `taskmark-frontend`.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |
| 2 | 2026-07-25T10:21:15Z | prompt | Marco Mendão | CLI must be `npx taskmark serve`; default port 8275 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

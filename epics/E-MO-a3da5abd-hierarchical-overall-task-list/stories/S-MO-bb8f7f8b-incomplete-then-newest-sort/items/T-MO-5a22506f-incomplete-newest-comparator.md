---
id: T-MO-5a22506f
type: task
title: Shared incomplete-then-newest sort comparator
status: backlog
priority: high
size: S
points: 3
parent: S-MO-bb8f7f8b
epic: E-MO-a3da5abd
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, overall]
created: 2026-08-29
updated: 2026-08-28T23:03:00Z
started_at: null
completed_at: null
---

# T-MO-5a22506f: Shared incomplete-then-newest sort comparator

## Description

Add a reusable comparator: incomplete statuses before complete/cancelled; then `created` descending; then `updated` descending; then id for stability.

## Acceptance criteria

- [ ] Comparator is unit-tested for mixed complete/incomplete and equal created dates.
- [ ] `done` and `cancelled` both sort after incomplete.


## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|


---
id: T-MO-8d7fbb62
type: task
title: Persist expanded Overall nodes in the session
status: done
priority: high
size: S
points: 3
parent: S-MO-6d9a5f48
epic: E-MO-a3da5abd
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
blocked: false
cancelled: false
tags: [dashboard, frontend, overall]
created: 2026-08-29
updated: 2026-08-28T23:17:07Z
started_at: 2026-08-28T23:15:42Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-8d7fbb62: Persist expanded Overall nodes in the session

## Description

Remember which epics and stories are expanded (sessionStorage or equivalent) so a refresh or sheet close does not fold the tree the user was using.

## Acceptance criteria

- [x] Expanded ids survive a client refresh in the same tab.
- [x] New visits can start collapsed except for URL deep links.


## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-28T23:07:00Z | prompt | Marco Mendão | /tkmd-do E-MO-a3da5abd: replace Overall stacked tables with one hierarchical tree (live+static); tests; no commit/push. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-28T23:15:42Z | 2026-08-28T23:16:11Z | Session-persist expanded epic/story ids. |


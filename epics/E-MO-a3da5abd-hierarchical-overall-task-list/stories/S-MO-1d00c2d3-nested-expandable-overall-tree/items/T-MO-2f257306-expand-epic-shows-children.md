---
id: T-MO-2f257306
type: task
title: Expand epic rows to stories and epic-direct items
status: done
priority: high
size: M
points: 5
parent: S-MO-1d00c2d3
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
started_at: 2026-08-28T23:09:54Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-2f257306: Expand epic rows to stories and epic-direct items

## Description

Epic rows are expandable. Open children are stories plus tasks/bugs whose parent is the epic (no story). Indent children under the epic.

## Acceptance criteria

- [x] Closed epics show a collapsed control; open epics show children immediately below.
- [x] Epic-direct tasks/bugs appear alongside stories under that epic.
- [x] General/optional epic behavior is unchanged if those epics still exist.


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
| Marco Mendão | 2026-08-28T23:09:54Z | 2026-08-28T23:10:23Z | Epic expand shows stories and epic-direct items in place. |


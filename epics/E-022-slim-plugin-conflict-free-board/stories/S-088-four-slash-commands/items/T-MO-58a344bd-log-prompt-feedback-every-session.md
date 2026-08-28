---
id: T-MO-58a344bd
type: task
title: Log prompt and feedback on every agent session
status: done
priority: high
size: S
points: 3
parent: S-088
epic: E-022
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
tags: [plugin, collaboration, board]
created: 2026-08-28
updated: 2026-08-28T22:37:36Z
started_at: 2026-08-28T22:36:27Z
completed_at: 2026-08-28T22:37:36Z
---

# T-MO-58a344bd: Log prompt and feedback on every agent session

## Description

Whenever an agent does product work, it must append Prompt & feedback on a
matching existing leaf (including a done task that still fits), or create a
new task/bug when nothing fits.

## Acceptance criteria

- [x] Conventions and `/tsmk-do` require a prompt row on the chosen leaf.
- [x] Prefer an open matching leaf, else a done leaf that still covers the work.
- [x] Create a new leaf only when no existing task/bug fits.
- [x] Never write Prompt & feedback on epic or story parent files.
- [x] Local plugin install is synced.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-28T22:36:27Z | prompt | Marco Mendão | Always write Prompt & feedback on a fitting done task, or create a new one. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-28T22:36:27Z | 2026-08-28T22:37:36Z | Added leaf Prompt & feedback session rules to conventions, tsmk-do, always-on memory, and docs. |

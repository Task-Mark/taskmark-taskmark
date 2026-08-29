---
id: T-MM-6884442c
type: task
title: Replace generated board-root README
status: done
priority: medium
size: S
points: 3
parent: S-MO-f7d1ac52
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [docs, readme]
created: 2026-08-29
updated: 2026-08-29T11:41:21Z
started_at: 2026-08-29T11:41:05Z
completed_at: 2026-08-29T11:41:21Z
---

# T-MM-6884442c: Replace generated board-root README

## Description

Cursor, plugin, frontend, website, and marketplace copy already describe the current slash set. The workspace/board-root README still publishes a generated Last-synced dashboard (Current speed, open-work table, changelog). Replace that with a short current-product README. Do not generate INDEX/SIZING/VELOCITY or a board README as product docs.

## Acceptance criteria

- [x] `taskmark-cursor` and plugin READMEs stay aligned with `/tkmd-*`, leaf-only writes, static sizing, and no INDEX/SIZING/VELOCITY/board README.
- [x] Workspace/board-root README no longer publishes Last synced, Current speed, or a generated open-work changelog as product documentation.
- [x] `taskmark-frontend` README remains accurate for `@taskmark/ui` install/serve and does not revive retired slash commands.
- [x] `taskmark-website` README points at landing + docs without contradicting the current command set.
- [x] Cursor marketplace plugin description matches the current commands if it is user-visible.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T11:37:37Z | prompt | Marco Mendão | Review E-MO-4b9b509e; most READMEs are current, but the board-root README is still a generated dashboard. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:41:05Z | 2026-08-29T11:41:21Z | Replaced generated workspace README; left plugin/frontend/website READMEs as current. |

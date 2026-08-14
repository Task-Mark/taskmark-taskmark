---
id: S-040
type: story
title: Capture git user on create and resolve
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 8
points_source: rolled_up
estimate_minutes: 130
actual_minutes: 2
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-011
epic: E-011
owner: ""
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
tags: [identity, git, plugin, skills]
created: 2026-07-23
updated: 2026-08-14T17:50:46.835Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 120000
---

# S-040: Capture git user on create and resolve

## User story

As a developer using Taskmark in Cursor, I want create and complete-work flows to stamp the current git config user so reporters and resolvers stay accurate without manual entry.

## Acceptance criteria

- [x] `create-epic` / `create-story` / `create-task` add the current git identity to `reporters` (and seed related activity author fields).
- [x] `complete-work` (and resolve path) adds the current git identity to `resolvers`.
- [x] Multiple distinct emails can accumulate on the same item; same email is merged (not duplicated).
- [x] Missing git config fails gracefully (empty identity / clear note) without blocking board writes.

## Tasks

- [T-114: Stamp reporter on create-* skills](items/T-114-stamp-reporter-on-create.md)
- [T-115: Stamp resolver on complete-work](items/T-115-stamp-resolver-on-complete.md)
- [T-116: Merge multi-author identity lists by email](items/T-116-merge-multi-author-by-email.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T17:28:57Z | prompt | Marco Mendão | Start developing E-011 (story scope). |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T17:28:57Z | 2026-07-23T17:28:57Z | rollup: children hold shared-batch; delivered story |

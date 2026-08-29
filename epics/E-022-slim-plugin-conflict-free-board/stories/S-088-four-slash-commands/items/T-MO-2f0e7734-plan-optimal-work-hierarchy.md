---
id: T-MO-2f0e7734
type: task
title: Plan the optimal Taskmark work hierarchy from prose
status: done
priority: high
size: L
points: 8
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
tags: [plugin, planning, hierarchy]
created: 2026-08-29
updated: 2026-08-29T10:48:48Z
started_at: 2026-08-29T10:44:15Z
completed_at: 2026-08-29T10:48:48Z
---

# T-MO-2f0e7734: Plan the optimal Taskmark work hierarchy from prose

## Description

Make `/tkmd-plan` reason from the user's requirements before writing files. It
must choose the smallest useful combination of epic, story, task, and bug,
split work into executable leaves, and avoid mechanically creating a new epic
for every prompt.

## Acceptance criteria

- [x] The skill classifies outcomes as epics, user-visible capabilities as stories, executable units as tasks, and defects/regressions as bugs.
- [x] It decomposes broad requests into cohesive stories and independently executable task/bug leaves with clear acceptance criteria.
- [x] It avoids oversized or duplicate items and uses static sizing to split work that is not sprint-ready.
- [x] It asks a question only when missing information would materially change the hierarchy or scope.
- [x] It reports the hierarchy and rationale concisely after writing the new item files.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:38:00Z | prompt | Marco Mendão | Rename `/tkmd-create` to `/tkmd-plan` and make it organize user requirements into the optimal Taskmark hierarchy. |
| 2026-08-29T10:42:00Z | prompt | Marco Mendão | `/tkmd-do`: complete every remaining task in S-088. |
| 2026-08-29T10:48:48Z | feedback | Marco Mendão | Added prose classification, minimal hierarchy design, sizing-driven decomposition and concise rationale reporting. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T10:44:15Z | 2026-08-29T10:46:30Z | Reworked tkmd-plan to decompose prose into cohesive, executable, statically sized hierarchy leaves. |

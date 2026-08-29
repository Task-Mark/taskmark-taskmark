---
id: T-MM-f84c1351
type: task
title: Refresh landing for the current product
status: done
priority: high
size: S
points: 3
parent: S-MO-60c97eed
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
tags: [website, landing]
created: 2026-08-29
updated: 2026-08-29T11:41:21Z
started_at: 2026-08-29T11:40:40Z
completed_at: 2026-08-29T11:41:05Z
---

# T-MM-f84c1351: Refresh landing for the current product

## Description

The landing console already uses `/tkmd-plan` / `/tkmd-do` / `/tkmd-commit`, but the board visual still shows an `in progress` badge and the effort feature still mentions idle/session-cap velocity. Update those surfaces so the page matches the current product without pretending there are only four commands.

## Acceptance criteria

- [x] Hero, console demo, and CTAs use current `/tkmd-*` names (not `/tkmd-create` or retired `/tsmk-*`).
- [x] Console demo IDs and outcomes look like current plan/do (collision-resistant IDs, implement without commit, explicit commit).
- [x] Features describe leaf-only writes, static XS–XXL points, Actual from closed work logs, and multi-repo `/tkmd-commit` — not idle/session-cap velocity or generated indexes.
- [x] Purpose/board visual shows nested epic → story → task without an `in_progress` badge as the product model.
- [x] Open-source and docs CTAs still resolve; metadata/SEO copy does not mention retired commands.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T11:37:37Z | prompt | Marco Mendão | Review E-MO-4b9b509e; landing still has leftover in-progress and session-cap copy. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:40:40Z | 2026-08-29T11:41:05Z | Dropped in-progress badge and session-cap copy; collision-resistant demo IDs. |

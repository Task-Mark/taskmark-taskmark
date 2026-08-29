---
id: T-MM-09761fd2
type: task
title: Align file spec with current leaf writes
status: done
priority: high
size: M
points: 5
parent: S-MO-4be0202b
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
tags: [docs, specification]
created: 2026-08-29
updated: 2026-08-29T11:41:21Z
started_at: 2026-08-29T11:38:20Z
completed_at: 2026-08-29T11:39:40Z
---

# T-MM-09761fd2: Align file spec with current leaf writes

## Description

The public file specification still shows retired frontmatter (`size_source` / `points_source`), short IDs without identity tokens, and leaf tables with a `#` column and Work log `Session` column. Update templates to match what `/tkmd-plan` writes today. Folder-structure docs already cover board layout; do not reintroduce a reserved General epic.

## Acceptance criteria

- [x] Frontmatter examples use current fields only (no estimate/owner; no `size_source` / `points_source`).
- [x] ID examples include `E|S|T|B-<identity>-<random>` and note that legacy `T-001`-style IDs remain valid.
- [x] Epic and story templates have no child lists, rollups, Prompt & feedback, Commits, or Work log.
- [x] Leaf table headings match conventions (`Prompt & feedback` without a `#` column; Work log Actor / Started / Ended / Summary).
- [x] Structure docs still cover single-repo `taskmark/` vs sibling `<common>-taskmark`, gitignored `REPOS.md`, and no INDEX/SIZING/VELOCITY/board README.
- [x] Docs do not tell readers to soft-attach to a reserved General epic.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T11:37:37Z | prompt | Marco Mendão | Review E-MO-4b9b509e; keep only work that still matches the current product. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:38:20Z | 2026-08-29T11:39:40Z | Rewrote spec templates to current IDs, frontmatter, and leaf tables. |

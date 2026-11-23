---
id: S-089
type: story
title: Stop committing INDEX, SIZING, VELOCITY, README, and REPOS
status: backlog
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 29
points_source: rolled_up
estimate_minutes: 290
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-022
epic: E-022
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, collaboration, board]
created: 2026-08-28
updated: 2026-08-28T12:37:43.783Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-089: Stop committing INDEX, SIZING, VELOCITY, README, and REPOS

## User story

As a teammate, I want generated board files out of git so that parallel plugin runs do not conflict on README, INDEX, SIZING, VELOCITY, or machine-local REPOS paths.

## Acceptance criteria

- [ ] Board git no longer tracks INDEX.md, SIZING.md, VELOCITY.md, README.md, or REPOS.md.
- [ ] REPOS.md is gitignored and generated locally by sync-taskmark-repos (absolute paths never pushed).
- [ ] No committed file gets a Last synced stamp or a git-log changelog.
- [ ] Init and sample board match the new file set.
- [ ] Board UI lists work by scanning `epics/` (query), not INDEX.md.

## Tasks

- [T-285: Stop writing INDEX.md; UI scans epics/](items/T-285-stop-writing-index.md)
- [T-286: Remove SIZING.md and VELOCITY.md generation](items/T-286-remove-sizing-velocity-files.md)
- [T-287: Delete board README.md and changelog dashboard](items/T-287-delete-readme-changelog.md)
- [T-288: Gitignore REPOS.md and generate it locally](items/T-288-gitignore-repos-md.md)
- [T-289: Stop Last synced timestamps in committed files](items/T-289-stop-last-synced.md)
- [T-290: Update init and sample board to the new file set](items/T-290-update-init-and-sample-board.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-28T12:19:14Z | prompt | Marco Mendão | Full housekeeping: slim commands, drop derived board files, static sizing, leaf-only MD, new IDs, delete unused plugin pieces. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

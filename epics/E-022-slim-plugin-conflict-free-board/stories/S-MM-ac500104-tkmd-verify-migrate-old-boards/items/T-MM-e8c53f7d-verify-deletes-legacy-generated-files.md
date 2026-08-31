---
id: T-MM-e8c53f7d
type: task
title: Verify deletes leftover generated board files
status: backlog
priority: high
size: S
points: 3
parent: S-MM-ac500104
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, migration, board]
created: 2026-08-31
updated: 2026-08-31T12:22:27Z
started_at: null
completed_at: null
---

# T-MM-e8c53f7d: Verify deletes leftover generated board files

At the canonical board root only, delete `INDEX.md`, `SIZING.md`, `VELOCITY.md`, and shared ID counter files (`NEXT_IDS` / `NEXT_IDS.md` and similar) when present. After the static README is in the correct place, delete a nested `taskmark/README.md` that is still a generated dashboard. Do not delete an existing `CHANGELOG.md`, `epics/`, `node_modules/`, or `out/`.

## Acceptance criteria

- [ ] `INDEX.md`, `SIZING.md`, and `VELOCITY.md` at the board root are removed when they exist.
- [ ] Shared ID counter files at the board root are removed when they exist.
- [ ] A nested generated dashboard README is removed only after the static project README lives in the init location.
- [ ] Existing `CHANGELOG.md` and `epics/` are left in place.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T12:22:27Z | prompt | Marco Mendão | Cursor plan: `/tkmd-verify` migrates old boards to the current Taskmark layout and item spec. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

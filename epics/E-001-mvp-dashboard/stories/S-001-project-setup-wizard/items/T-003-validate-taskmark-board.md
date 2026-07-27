---
id: T-003
type: task
title: Validate taskmark board in selected folder
status: done
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 2
estimate_basis: [calibrated:T-003]
session_cap_minutes: 480
parent: S-001
epic: E-001
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
tags: [mvp, wizard, validation]
created: 2026-07-21
updated: 2026-07-27T05:18:44.416Z
started_at: 2026-07-21T16:35:18Z
completed_at: 2026-07-21T16:37:18Z
actual_ms: 120000
---
# T-003: Validate taskmark board in selected folder

## Description

After the user selects a **master folder**, verify it is usable: the path exists and is readable, and discovery finds **at least one** Taskmark project in its subfolders (via T-008). Do **not** require `taskmark/` at the master root. Surface clear errors for unreadable path vs no projects found.

## Acceptance criteria

- [x] Master folder that yields ≥1 discovered Taskmark project passes validation.
- [x] Missing/unreadable path shows a specific error message.
- [x] Readable master with zero discovered boards shows a clear “no Taskmark projects found” error.
- [x] Validation is callable from the wizard before persist/continue.
- [x] Does not mutate board files.

## Notes

Keep checks lightweight for MVP; deep schema validation can come later. Relies on discovery (T-008).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T16:24:55Z | prompt | Marco Mendão | Create MVP epic with setup wizard + epic list; create stories and tasks |
| 2 | 2026-07-21T16:31:04Z | feedback | Marco Mendão | Validate master folder via subfolder discovery, not only root taskmark/ |
| 3 | 2026-07-21T16:37:18Z | prompt | Marco Mendão | Implement S-001 setup wizard |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T16:05:18Z | 2026-07-21T16:07:18Z | auto-backfilled: velocity × points (missing work log); shared-batch: 2 of 4min by points |

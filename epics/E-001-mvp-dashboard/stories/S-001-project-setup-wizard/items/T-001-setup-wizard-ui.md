---
id: T-001
type: task
title: Build setup wizard UI shell
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_basis: [calibrated:T-001]
session_cap_minutes: 480
parent: S-001
epic: E-001
owner: ""
blocked: false
cancelled: false
tags: [mvp, wizard, ui]
created: 2026-07-21
updated: 2026-07-23T16:33:36.080Z
started_at: 2026-07-21T16:35:18Z
completed_at: 2026-07-21T16:37:18Z
actual_ms: 180000
---
# T-001: Build setup wizard UI shell

## Description

Create the first-run setup wizard layout and steps shell in the frontend: welcome copy, primary CTA to choose a project, and a placeholder for folder selection / validation messages. Route or gate the home experience so users without a saved project land on the wizard.

## Acceptance criteria

- [x] App shows a dedicated setup wizard when no project is selected.
- [x] Wizard includes clear product framing and a single primary path to select a folder.
- [x] Layout works on desktop and mobile widths.
- [x] Existing UI primitives (button, etc.) are reused where they fit.

## Notes

Part of MVP scope for E-001; full dashboard beyond wizard + epic list is out of scope for this epic slice.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T16:24:55Z | prompt | Create MVP epic with setup wizard + epic list; create stories and tasks |
| 2 | 2026-07-21T16:37:18Z | prompt | Implement S-001 setup wizard |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T15:49:18Z | 2026-07-21T15:52:18Z | auto-backfilled: velocity × points (missing work log); shared-batch: 3 of 6min by points |

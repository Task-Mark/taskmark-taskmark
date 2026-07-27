---
id: T-004
type: task
title: Persist selected project and enter app
status: done
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 2
estimate_basis: [calibrated:T-004]
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
tags: [mvp, wizard, persistence]
created: 2026-07-21
updated: 2026-07-27T05:30:10.150Z
started_at: 2026-07-21T16:35:18Z
completed_at: 2026-07-21T16:37:18Z
actual_ms: 120000
---

# T-004: Persist selected project and enter app

## Description

On successful validation, store the selected **master folder** path in a **cookie** and navigate the user into the main app surface (epic lists for discovered projects). On subsequent launches, if the cookie holds a master folder path, skip the setup wizard and go straight to the app. Users who already set up must not be forced through setup again. Provide a clear path back into the setup wizard to **switch** master folders and overwrite the cookie.

## Acceptance criteria

- [x] Valid master folder path is stored in a cookie (not localStorage) and survives reload / browser restart for the cookie’s lifetime.
- [x] Returning users with a master-folder cookie skip the setup wizard and enter the app directly.
- [x] After first successful setup, the user is not required to set up again unless they choose to switch or the cookie is missing/invalid.
- [x] After save, user lands on the epic list surface for projects discovered under that master folder.
- [x] Saved invalid/missing path (or master with no discoverable projects) clears or ignores the cookie and falls back to the wizard with an explanation.
- [x] User can open setup again to switch master folders; confirming a new valid folder updates the cookie.

## Notes

Cookie name `taskmark_master_folder`, httpOnly, maxAge 1 year, stores master folder path.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T16:24:55Z | prompt | Marco Mendão | Create MVP epic with setup wizard + epic list; create stories and tasks |
| 2 | 2026-07-21T16:29:20Z | feedback | Marco Mendão | Persist project in cookies; skip setup when already configured; allow switching projects via setup |
| 3 | 2026-07-21T16:31:04Z | feedback | Marco Mendão | Cookie stores master folder; multiple Taskmark projects live in subfolders |
| 4 | 2026-07-21T16:37:18Z | prompt | Marco Mendão | Implement S-001 setup wizard |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T16:05:18Z | 2026-07-21T16:07:18Z | auto-backfilled: velocity × points (missing work log); shared-batch: 2 of 4min by points |

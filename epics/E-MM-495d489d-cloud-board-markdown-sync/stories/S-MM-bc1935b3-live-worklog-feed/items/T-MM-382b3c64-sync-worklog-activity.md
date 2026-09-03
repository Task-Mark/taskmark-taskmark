---
id: T-MM-382b3c64
type: task
title: Send new worklog activity during board sync
status: done
priority: high
size: M
points: 5
parent: S-MM-bc1935b3
epic: E-MM-495d489d
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
tags: [cli, sync, worklog]
created: 2026-09-03
updated: 2026-09-03T18:54:00Z
started_at: 2026-09-03T18:41:51Z
completed_at: 2026-09-03T18:54:00Z
---
# T-MM-382b3c64: Send new worklog activity during board sync

## Description

Use the existing local markdown watcher to detect newly added leaf work-log rows and attach compact activity events to the final board-sync batch.

## Acceptance criteria

- [x] Activity is extracted only from task and bug details.
- [x] Stable fingerprints prevent repeated events within one watcher process.
- [x] Initial startup seeds fingerprints without replaying historical work logs.
- [x] New activity travels through the existing token-authenticated board-sync request.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T18:41:51Z | prompt | Marco Mendão | Save and implement local polling that sends new work logs through Cloud sync. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T18:41:51Z | 2026-09-03T18:54:00Z | Attached new leaf work-log events to the final board-sync batch. |

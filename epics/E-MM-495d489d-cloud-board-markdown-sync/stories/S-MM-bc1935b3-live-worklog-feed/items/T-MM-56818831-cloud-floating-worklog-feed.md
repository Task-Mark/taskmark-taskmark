---
id: T-MM-56818831
type: task
title: Show the floating worklog feed on Cloud
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
tags: [cloud, ui, polling, worklog]
created: 2026-09-03
updated: 2026-09-03T18:54:00Z
started_at: 2026-09-03T18:41:51Z
completed_at: 2026-09-03T18:54:00Z
---
# T-MM-56818831: Show the floating worklog feed on Cloud

## Description

Poll recent project work-log activity and display it in the shared floating message feed while the full board continues to refresh from board versions.

## Acceptance criteria

- [x] Cloud polls project activity without reloading the full snapshot.
- [x] Floating messages appear at the right of the board, expire after five minutes, and never exceed six.
- [x] A seventh message evicts the oldest visible message.
- [x] Board version polling continues to refresh every board view automatically.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T18:54:00Z | prompt | Marco Mendão | Play soundcn bong-001 whenever a new Cloud work-log message appears. |
| 2026-09-03T18:41:51Z | prompt | Marco Mendão | Save and implement a floating Cloud developer work feed with six-message FIFO and five-minute expiry. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T18:41:51Z | 2026-09-03T18:54:00Z | Polled Cloud activity into the floating feed and played bong-001 for each new message. |

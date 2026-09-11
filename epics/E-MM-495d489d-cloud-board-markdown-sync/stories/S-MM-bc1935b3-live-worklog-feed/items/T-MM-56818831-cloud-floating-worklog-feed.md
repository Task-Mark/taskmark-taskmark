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
tags: [cloud, ui, sse, worklog]
created: 2026-09-03
updated: 2026-09-07T19:43:28Z
started_at: 2026-09-03T18:41:51Z
completed_at: 2026-09-07T19:43:28Z
---
# T-MM-56818831: Show the floating worklog feed on Cloud

## Description

Stream recent project work-log activity, presence summaries, and board versions over one authenticated Server-Sent Events connection. Display worklogs in the shared floating message feed and refresh the full board when its streamed version changes.

## Acceptance criteria

- [x] Cloud receives project activity and presence summaries over a shared SSE connection without reloading the full snapshot.
- [x] Floating messages appear at the right of the board, expire after five minutes, and never exceed six.
- [x] A seventh message evicts the oldest visible message.
- [x] Streamed board version changes refresh every board view automatically.
- [x] The SSE stream is authenticated, exempt from request throttling, and kept alive with heartbeat events.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-07T19:43:28Z | prompt | Marco Mendão | Replace repeated worklog, presence, and board-version polling with Server-Sent Events to eliminate throttling errors. |
| 2026-09-03T18:54:00Z | prompt | Marco Mendão | Play soundcn bong-001 whenever a new Cloud work-log message appears. |
| 2026-09-03T18:41:51Z | prompt | Marco Mendão | Save and implement a floating Cloud developer work feed with six-message FIFO and five-minute expiry. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-07T19:36:00Z | 2026-09-07T19:43:28Z | Replaced three Cloud polling loops with one authenticated SSE stream for board versions, worklogs, and presence summaries. |
| Marco Mendão | 2026-09-03T18:41:51Z | 2026-09-03T18:54:00Z | Polled Cloud activity into the floating feed and played bong-001 for each new message. |

---
id: T-MM-a9765753
type: task
title: Add shared worklog feed components
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
tags: [ui, components, shadcn, worklog]
created: 2026-09-03
updated: 2026-09-03T19:05:00Z
started_at: 2026-09-03T18:41:51Z
completed_at: 2026-09-03T18:54:00Z
---
# T-MM-a9765753: Add shared worklog feed components

## Description

Install the shadcn Message and Bubble primitives in `@taskmark/components`, then compose reusable work-activity messages and a full Worklog panel.

## Acceptance criteria

- [x] `npx shadcn@latest add message bubble` installs compatible shared primitives.
- [x] A shared floating activity component renders actor, item, summary, and time with existing avatar styling.
- [x] The floating component keeps at most six messages, expires them after five minutes, and evicts the oldest first.
- [x] A shared Worklog panel renders complete leaf work-log history newest first.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T19:05:00Z | prompt | Marco Mendão | Make the feed avatar larger and top-aligned; show only a work-item code tag with a title tooltip. |
| 2026-09-03T18:54:00Z | prompt | Marco Mendão | Play soundcn bong-001 whenever a new work-log message appears. |
| 2026-09-03T18:41:51Z | prompt | Marco Mendão | Save and implement the plan for shadcn worklog messages and a shared Worklog panel. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T19:05:00Z | 2026-09-03T19:05:00Z | Aligned a larger feed avatar to the top of each card and replaced the item title with a typed code tag plus tooltip. |
| Marco Mendão | 2026-09-03T18:41:51Z | 2026-09-03T18:54:00Z | Added Message/Bubble, WorkActivityFeed, WorklogPanel, and bong-001 playback for new feed messages. |

---
id: T-MM-b6bdc358
type: task
title: Contributor leaderboard for the filtered period
status: backlog
priority: medium
size: M
points: 5
parent: S-MM-07de76ad
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, leaderboard]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-b6bdc358: Contributor leaderboard for the filtered period

## Description

Rank contributors within the filtered period: points completed (from completion samples attributed to each resolver) and number of worklog sessions (from the merged worklog rows per actor). Render with `ActorAvatar`, position number, and both metrics; ties break by session count. Respects all global filters.

## Acceptance criteria

- [ ] Contributors are ranked by points completed in the filtered period, with session counts shown alongside.
- [ ] Points attribution uses the completion samples' resolvers; sessions come from worklog actors.
- [ ] The leaderboard honours project, author, and timeframe filters.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — contributor leaderboard by points and sessions. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

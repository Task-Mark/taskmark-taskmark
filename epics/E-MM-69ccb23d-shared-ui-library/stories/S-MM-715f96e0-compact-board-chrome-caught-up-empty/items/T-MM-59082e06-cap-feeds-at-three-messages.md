---
id: T-MM-59082e06
type: task
title: Cap worklog and presence feeds at three messages
status: done
priority: high
size: XS
points: 1
parent: S-MM-715f96e0
epic: E-MM-69ccb23d
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
tags: [ui, worklog, presence]
created: 2026-09-15
updated: 2026-09-15T22:28:00Z
started_at: 2026-09-15T22:11:00Z
completed_at: 2026-09-15T22:28:00Z
---
# T-MM-59082e06: Cap worklog and presence feeds at three messages

## Description

Keep at most three floating worklog messages and three presence summary messages. Evict the oldest card when a newer one arrives.

## Acceptance criteria

- [x] The worklog activity feed shows at most three messages and evicts the oldest first.
- [x] The presence summary feed shows at most three cards and evicts the oldest first.
- [x] The cap applies on local, npx static, and Cloud boards wherever those feeds render.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T22:11:00Z | prompt | Marco Mendão | Allow at most three worklog messages and three summary messages on every board. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T22:11:00Z | 2026-09-15T22:28:00Z | Capped worklog and presence feeds at three visible cards. |

---
id: S-MM-715f96e0
type: story
title: Compact board chrome and caught-up empty states
status: backlog
priority: high
size: null
points: null
parent: E-MM-69ccb23d
epic: E-MM-69ccb23d
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [ui, board, worklog, empty-state]
created: 2026-09-15
updated: 2026-09-15T22:11:00Z
started_at: null
completed_at: null
---
# S-MM-715f96e0: Compact board chrome and caught-up empty states

## Description

Polish the shared board UI so Overall and Work items show a clear caught-up empty state, floating worklog and presence chrome stays compact (three messages each, collapsible until hover), the worklog count card shows daily totals, and each worklog bubble places the item tag at the bottom right. The same chrome must appear on local, npx, and Cloud boards.

## User story

As a board user, I want a quieter board when work is done and when activity chrome is in the way, so I can scan remaining work and still peek at live messages and counts when I need them.

## Acceptance criteria

- [ ] Overall and Work items show a distinct empty state when there is no remaining open work.
- [ ] Floating worklog messages and presence summaries each show at most three cards.
- [ ] A control minimizes the messages and the worklog count card; after that they expand only on hover.
- [ ] The speedometer day list shows how many work logs were recorded each day.
- [ ] The worklog message item tag sits at the bottom right of the bubble.
- [ ] Local, npx static, and Cloud boards share this behavior through `@taskmark/components`.

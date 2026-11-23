---
id: S-MM-1318bfdd
type: story
title: Reports tab in the board UI
status: backlog
priority: high
size: null
points: null
parent: E-MM-5a80f20a
epic: E-MM-5a80f20a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, reports, ui]
created: 2026-08-31
updated: 2026-08-31T06:47:12Z
started_at: null
completed_at: null
---

# S-MM-1318bfdd: Reports tab in the board UI

## User story

As someone using the local board UI, I want a Reports tab with a dropdown of every report on the system, so I can open the newest one immediately and still go back to an older one when I need it.

## Acceptance criteria

- [ ] The board UI has a Reports tab that renders the selected report's markdown
- [ ] A dropdown lists every `.reports/report-YYYYMMDD.md` file, newest first
- [ ] The newest report is selected by default when the tab opens
- [ ] The tab is absent when no report exists, and `?view=reports` then falls back to the default list view
- [ ] Live `taskmark serve` / `dev` and static snapshot builds behave identically
- [ ] Writing a new report while `taskmark dev` is running refreshes the board without a manual reload

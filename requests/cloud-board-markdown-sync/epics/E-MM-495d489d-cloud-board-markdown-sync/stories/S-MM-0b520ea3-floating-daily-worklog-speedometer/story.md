---
id: S-MM-0b520ea3
type: story
title: Floating daily worklog speedometer on Cloud
status: backlog
priority: high
size: null
points: null
parent: E-MM-495d489d
epic: E-MM-495d489d
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, worklog, ui, gauge]
created: 2026-09-03
updated: 2026-09-03T19:55:00Z
started_at: null
completed_at: null
---
# S-MM-0b520ea3: Floating daily worklog speedometer on Cloud

## Description

Show a floating left-side speedometer on the Cloud board that tracks how many work-log sessions the team recorded today, scaled against the busiest day in the last 30 days.

## User story

As a Cloud teammate looking at the board, I want a live daily work-log speedometer so I can see whether today is keeping up with our recent busiest day.

## Acceptance criteria

- [ ] Cloud shows a floating speedometer on the left, matching the floating worklog feed on the right.
- [ ] The gauge value is today's work-log count; the maximum is the highest daily count in the last 30 days.
- [ ] The center icon follows the daily mood and end-of-day flame rules.

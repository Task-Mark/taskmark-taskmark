---
id: T-MM-0ba28f99
type: task
title: Count today against a 30-day worklog peak
status: done
priority: high
size: S
points: 3
parent: S-MM-0b520ea3
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
tags: [worklog, metrics]
created: 2026-09-03
updated: 2026-09-15T22:46:00Z
started_at: 2026-09-03T19:55:00Z
completed_at: 2026-09-03T20:10:00Z
---
# T-MM-0ba28f99: Count today against a 30-day worklog peak

## Description

From flattened leaf work-log rows, count sessions per local calendar day using the started timestamp. Today's count is the gauge value. The maximum is the largest daily count in a rolling 10-day window that includes today. If that window has no sessions, the peak is the count from the last day anyone worked on the project.

## Acceptance criteria

- [x] Leaf work-log rows are grouped by local calendar day of `started`.
- [x] The lookback is the last 10 local days, including today.
- [x] Peak is the maximum daily count in that window; if the window is idle, peak is the last worked day in the project.
- [x] Today is the count for the current local day.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T22:46:00Z | prompt | Marco Mendão | Use a 10-day worklog peak, and if those days are idle fall back to the last day worked on the project. |
| 2026-09-03T19:55:00Z | prompt | Marco Mendão | Count today's work logs against the busiest of the last 30 days for a Cloud speedometer. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T22:46:00Z | 2026-09-15T22:46:00Z | Switched the speedometer peak to 10 days, with a last-worked-day fallback. |
| Marco Mendão | 2026-09-03T19:55:00Z | 2026-09-03T20:10:00Z | Added local-day work-log counts and a 30-day peak for the Cloud speedometer. |

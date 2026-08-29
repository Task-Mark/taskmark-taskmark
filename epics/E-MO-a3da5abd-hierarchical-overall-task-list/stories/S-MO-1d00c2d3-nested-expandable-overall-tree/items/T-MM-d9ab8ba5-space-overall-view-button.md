---
id: T-MM-d9ab8ba5
type: task
title: Space Overall view button away from status
status: done
priority: medium
size: XS
points: 1
parent: S-MO-1d00c2d3
epic: E-MO-a3da5abd
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
tags: [dashboard, frontend, overall, ux]
created: 2026-08-29
updated: 2026-08-29T17:11:15Z
started_at: 2026-08-29T17:10:49Z
completed_at: 2026-08-29T17:11:15Z
---

# T-MM-d9ab8ba5: Space Overall view button away from status

## Description

On Overall, the view-work-item eye sits flush against the status (or progress) control. Add margin so the button is not stuck to that chrome. Follow-up on T-MO-b91943ff; do not change All / Stories / Tasks unless they share this row.

## Acceptance criteria

- [x] Overall tree view button has visible space from the status or child-progress control
- [x] Opening the sheet from that button still works
- [x] Other Overall row chrome (type, title, expand) is unchanged

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:10:49Z | prompt | Marco Mendão | `/tkmd-plan-do`: Overall view-work-item button needs margin so it is not stuck to the work-item status. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T17:10:49Z | 2026-08-29T17:11:15Z | Added Overall view-button padding and wider last columns. |

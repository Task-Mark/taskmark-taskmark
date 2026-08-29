---
id: T-MO-809fcbb3
type: task
title: Hide completed without hiding open descendant work
status: done
priority: high
size: M
points: 5
parent: S-MO-3a71914c
epic: E-MO-a3da5abd
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
blocked: false
cancelled: false
tags: [dashboard, frontend, overall]
created: 2026-08-29
updated: 2026-08-28T23:26:51Z
started_at: 2026-08-28T23:14:15Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-809fcbb3: Hide completed without hiding open descendant work

## Description

Hide-completed removes completed leaves and completed parents that have no remaining visible descendants. A completed epic/story with incomplete children stays visible.

## Acceptance criteria

- [x] Completed tasks hide when the toggle is on.
- [x] A done epic with an incomplete story still appears.
- [x] Preference persistence matches existing hide-completed cookies/keys as far as practical.
- [x] Toggling hide-completed keeps the user's expanded and collapsed nodes.


## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-28T23:07:00Z | prompt | Marco Mendão | /tkmd-do E-MO-a3da5abd: replace Overall stacked tables with one hierarchical tree (live+static); tests; no commit/push. |
| 2026-08-28T23:24:00Z | prompt | Marco Mendão | Hide completed expands every task; open nodes should stay open and collapsed nodes stay collapsed. |
| 2026-08-28T23:26:51Z | feedback | Marco Mendão | Only a search now reveals ancestors; hide-completed and timeframe preserve expansion state. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-28T23:14:15Z | 2026-08-28T23:14:44Z | Hide-completed keeps completed ancestors with incomplete descendants. |
| Marco Mendão | 2026-08-28T23:24:00Z | 2026-08-28T23:26:51Z | Restricted auto-expansion to search so filter toggles keep expansion state; added regression test. |


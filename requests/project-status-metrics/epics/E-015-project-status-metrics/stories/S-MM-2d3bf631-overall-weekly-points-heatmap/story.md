---
id: S-MM-2d3bf631
type: story
title: Weekly story-points heatmap on Overall
status: backlog
priority: high
size: null
points: null
parent: E-015
epic: E-015
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, overall, metrics, ux]
created: 2026-08-29
updated: 2026-08-29T17:46:00Z
started_at: null
completed_at: null
---

# S-MM-2d3bf631: Weekly story-points heatmap on Overall

## User story

As a board user, I want a contribution-style heatmap on Overall that shows how many story points were completed each week, so I can scan throughput over time without reading the tree or the speed card.

## Acceptance criteria

- [ ] Overall (live and static) shows a heatmap inspired by a GitHub-style week calendar (reference: 8StarLabs Heatmap), placed above the hierarchical tree.
- [ ] Each cell is one ISO week; its value is the sum of story points from **done** task/bug leaves completed that week (`completed_at`). Parents are not double-counted. Shelved and cancelled leaves are excluded.
- [ ] Visual language matches the board’s retro / neo-brutalist metrics (hard borders, offset shadows, discrete palette) rather than a generic GitHub green clone.
- [ ] Hover or focus shows the week range and point total; empty weeks and boards with no done leaves are readable; the control is usable on desktop and a typical mobile width.
- [ ] The heatmap does not replace or break the Overall tree, search, hide-completed, or timeframe filter.

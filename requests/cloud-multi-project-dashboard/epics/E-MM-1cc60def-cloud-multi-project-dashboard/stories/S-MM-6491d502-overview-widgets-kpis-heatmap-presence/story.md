---
id: S-MM-6491d502
type: story
title: Overview widgets — KPIs, contribution heatmap, team summaries
status: backlog
priority: high
size: null
points: null
parent: E-MM-1cc60def
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, dashboard, widgets, presence]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# S-MM-6491d502: Overview widgets — KPIs, contribution heatmap, team summaries

## Description

The top of the dashboard answers "how are we doing" at a glance: a KPI strip built from `MetricStatCard`, a contribution heatmap reusing `PointsHeatmap` fed by author-aware completion samples, and the AI presence summaries grouped by project so each team's current focus reads like a status board.

## User story

As a Cloud user, I want headline numbers, a contribution calendar, and short summaries of what each person is doing per team so I understand the state of all projects in seconds.

## Acceptance criteria

- [ ] A KPI strip shows active projects, tasks in progress, points completed this week, worklog sessions in the period, and active contributors.
- [ ] The contribution heatmap aggregates completions across projects and narrows correctly by author, project, and timeframe.
- [ ] Presence summaries appear grouped by project, one card per person, matching the tone of the per-board presence feed.

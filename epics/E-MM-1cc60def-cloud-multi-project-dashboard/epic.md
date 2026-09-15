---
id: E-MM-1cc60def
type: epic
title: Cloud multi-project dashboard
status: backlog
priority: high
size: null
points: null
parent: null
epic: null
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, dashboard, api, analytics]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# E-MM-1cc60def: Cloud multi-project dashboard

## Description

Add a `/dashboard` route to Taskmark Cloud with an aggregated view of every project the signed-in user belongs to: worklogs across projects, AI presence summaries per team, a contribution heatmap filterable by author and project, active tasks everywhere, project health cards, and insight widgets (leaderboard, velocity comparison, task-vs-bug split). The view is backed by a new compact `GET /dashboard` aggregation endpoint on taskmark-api so the browser never downloads full 8 MB board snapshots per project.

```mermaid
flowchart LR
  subgraph api [taskmark-api]
    BoardState[(BoardState per project)]
    DashSvc[DashboardService extracts compact payload]
    BoardState --> DashSvc
  end
  subgraph cloud [taskmark-cloud]
    Page[app/dashboard/page.tsx server component]
    Filters[Client filters: project, author, timeframe]
    Widgets[KPIs, heatmap, worklogs, active tasks, presence]
  end
  DashSvc -->|"GET /dashboard"| Page --> Filters --> Widgets
```

## Goal

A member opens one Cloud page and sees, across all their projects at once, who is working on what, the work logged recently, points completed over time, and which tasks are active — with filters by author, project, and timeframe.

## Acceptance criteria

- [ ] A `/dashboard` route aggregates every active project of the signed-in user without fetching full board snapshots in the browser.
- [ ] Worklogs, presence summaries, contribution heatmap, active tasks, and project health are all visible on one page.
- [ ] Global filters by project, author, and timeframe apply to every widget.
- [ ] The dashboard is reachable from the Cloud app bar and mobile menu.

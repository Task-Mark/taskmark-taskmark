---
id: S-MO-2a76e28a
type: story
title: Document Overall tree and board UI
status: backlog
priority: high
size: M
points: 5
parent: E-MO-4b9b509e
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [docs, website, overall]
created: 2026-08-28
updated: 2026-08-28T23:15:25Z
started_at: null
completed_at: null
---

# S-MO-2a76e28a: Document Overall tree and board UI

## User story

As a board user, I want docs (and landing where it helps) to describe Overall as one nested list and to explain that parent status, points, people, dates, and logs are read-time views so the UI matches how the plugin writes markdown.

## Acceptance criteria

- [ ] Docs explain Overall as a hierarchical tree: expand epic → stories and epic-direct work; expand story → tasks/bugs; incomplete then newest at each level.
- [ ] Docs note that All, Stories, and Tasks views stay flat lists, and that search, hide-completed, timeframe, pagination, and deep links apply to the tree.
- [ ] Docs explain derived parent views (status, points, Actual, implementers, lifecycle dates, aggregated logs) vs leaf-only writes.
- [ ] How to open the local board (`@taskmark/ui`, bound vs workspace) is accurate relative to the frontend README.
- [ ] Landing or docs do not show Overall as three stacked independent tables.

---
id: S-MM-0af86fe8
type: story
title: Render Mermaid diagrams in work item detail
status: backlog
priority: high
size: null
points: null
parent: E-005
epic: E-005
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, markdown, mermaid]
created: 2026-08-29
updated: 2026-08-29T17:04:26Z
started_at: null
completed_at: null
---

# S-MM-0af86fe8: Render Mermaid diagrams in work item detail

## User story

As a board user, I want fenced Mermaid blocks in epic, story, and task markdown to show as diagrams so I can read AI-generated flowcharts without decoding the source.

## Acceptance criteria

- [ ] Fenced `mermaid` blocks in work-item detail prose render as diagrams
- [ ] Other fenced languages stay as formatted code
- [ ] Invalid diagrams do not crash the sheet

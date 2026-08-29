---
id: T-MM-fd09602a
type: task
title: Render mermaid code fences as diagrams in the detail sheet
status: done
priority: high
size: M
points: 5
parent: S-MM-0af86fe8
epic: E-005
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
tags: [frontend, markdown, mermaid]
created: 2026-08-29
updated: 2026-08-29T17:07:04Z
started_at: 2026-08-29T17:04:26Z
completed_at: 2026-08-29T17:07:04Z
---

# T-MM-fd09602a: Render mermaid code fences as diagrams in the detail sheet

## Description

`MarkdownContent` currently treats ```mermaid as a normal code block. Render those fences as diagrams in the work item sheet (goal, description, and other prose that uses MarkdownContent). Fit under E-005; do not reopen T-086.

## Acceptance criteria

- [x] ` ```mermaid ` fences in detail prose render as SVG/diagrams (flowchart, sequence, and similar Mermaid types)
- [x] Non-mermaid fenced code still renders as code
- [x] A broken diagram shows a readable error or source instead of crashing the sheet
- [x] Diagrams are readable in the sheet (scroll/overflow) and follow light/dark page colors when the UI uses them

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:04:26Z | prompt | Marco Mendão | `/tkmd-plan-do`: add Mermaid so AI-generated flowcharts and other graphics can be read on the board. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T17:04:26Z | 2026-08-29T17:07:04Z | Render mermaid fences in MarkdownContent; mermaid dependency; error fallback. |

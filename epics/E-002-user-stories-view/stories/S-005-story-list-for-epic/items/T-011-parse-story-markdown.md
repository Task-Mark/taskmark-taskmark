---
id: T-011
type: task
title: Parse story markdown under selected epic
status: done
priority: high
size: XS
size_source: suggested
size_basis: [calibrated:T-011]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 15
estimate_basis: [calibrated:T-011]
session_cap_minutes: 480
parent: S-005
epic: E-002
owner: ""
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
tags: [parser, stories]
created: 2026-07-21
updated: 2026-07-27T07:45:28.202Z
started_at: 2026-07-21T17:45:49Z
completed_at: 2026-07-21T17:48:46Z
actual_ms: 907000
---

# T-011: Parse story markdown under selected epic

## Description

Extend the board reader so that, given a project board path and an epic id (or epic folder), it scans `taskmark/epics/{epic}/stories/*/story.md`, parses YAML frontmatter and key fields (id, title, status, size, points, estimate_minutes, actual_minutes, priority, tags, parent), and returns a typed list of stories for that epic.

## Acceptance criteria

- [x] Discovers all story folders with a `story.md` under the selected epic.
- [x] Returns structured story summaries suitable for a list view.
- [x] Malformed files are skipped or flagged without failing the whole scan.
- [x] Works against real Taskmark boards in this workspace.

## Notes

Mirror the epic parser pattern from T-005; keep the API consistent for later task parsing (T-014).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T17:40:05Z | prompt | Marco Mendão | Create E-002 user stories view with stories and tasks |
| 2 | 2026-07-21T17:45:49Z | prompt | Marco Mendão | Start developing S-005 (includes this task) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 0c104cd | taskmark-frontend | 2026-07-21T17:59:56Z | Marco Mendão | add story list for selected epic |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T17:45:49Z | 2026-07-21T17:46:49Z | Parsed story.md under selected epic; shared frontmatter helpers; shared-batch: 1 of 1min by points |
| 2 | Marco Mendão | 2026-07-21T17:45:49Z | 2026-07-21T17:59:56Z | auto-recovered: commit span; shared-batch: 5 of 14min by points |

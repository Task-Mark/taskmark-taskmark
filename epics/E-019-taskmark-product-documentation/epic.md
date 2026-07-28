---
id: E-019
type: epic
title: Taskmark product documentation
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 58
points_source: rolled_up
estimate_minutes: 765
actual_minutes: 13
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
tags: [docs, website, documentation]
created: 2026-07-28
updated: 2026-07-28T08:51:45Z
started_at: 2026-07-28T07:43:14Z
completed_at: 2026-07-28T08:05:14Z
actual_ms: 780000
---

# E-019: Taskmark product documentation

## Goal

Ship comprehensive Taskmark product documentation on `taskmark-website` covering setup, slash commands, board layout, sizing, velocity, the README dashboard, and related day-to-day workflows.

## Scope

- Documentation information architecture and navigation
- Setup / install / first board
- Commands reference (`/new-epic`, `/new-story`, `/new-task` and create-* skills; `/start-work`; `/commit-all`; remaining sync/utility commands)
- Folder structure (single- and multi-repo)
- T-shirt sizing and story points
- Velocity (Current Speed, ETA, estimate intensity)
- README dashboard contents and refresh automation
- Work logs, multi-repo workflow, prompt/feedback and commits logs

## Out of scope

- Translating docs to other languages
- Full API reference for internal Python scripts beyond user-facing behavior
- Hosting/infra for docs (CDN, search SaaS)

## Success metrics

- All scoped topics published under the docs area
- Commands documented with correct slash names and effects
- Visitors can go from install → first board → core loop without leaving docs

## Stories

- [S-072: Docs information architecture and navigation](stories/S-072-docs-information-architecture/story.md)
- [S-073: Setup and installation guide](stories/S-073-setup-and-installation-guide/story.md)
- [S-074: Slash commands reference](stories/S-074-slash-commands-reference/story.md)
- [S-075: Board folder structure](stories/S-075-board-folder-structure/story.md)
- [S-076: Sizing and story points](stories/S-076-sizing-and-story-points/story.md)
- [S-077: Velocity and ETA](stories/S-077-velocity-and-eta/story.md)
- [S-078: README dashboard](stories/S-078-readme-dashboard/story.md)
- [S-079: Core workflows and related topics](stories/S-079-core-workflows-and-related-topics/story.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T07:40:05Z | prompt | Marco Mendão | Create documentation epic covering setup, commands (/create-epic, /create-task, /create-story, /start-work, /commit-all and others), folder structure, sizing and story points, velocity, README dashboard, and related topics; create stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4d10e86 | taskmark-taskmark | 2026-07-28T08:51:45Z | Marco Mendão | log E-014 and E-019 commits |
| 783fa2d | taskmark-website | 2026-07-28T09:50:48Z | Marco Mendão | add docs site pages and file specification |
| 935c164 | taskmark-taskmark | 2026-07-28T09:50:56Z | Marco Mendão | sync taskmark board |
| 31a2da5 | taskmark-taskmark | 2026-07-28T07:42:10Z | Marco Mendão | add e-019 documentation epic |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T07:43:14Z | 2026-07-28T07:43:14Z | shared-batch rollup: leaves hold billable minutes for docs delivery |

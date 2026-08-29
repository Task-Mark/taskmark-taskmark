---
id: T-MM-f6d018dc
type: task
title: Agent markdown always uses the stored board language
status: backlog
priority: high
size: M
points: 5
parent: S-MM-9bcdb844
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, conventions, i18n]
created: 2026-08-29
updated: 2026-08-29T17:29:52Z
started_at: null
completed_at: null
---

# T-MM-f6d018dc: Agent markdown always uses the stored board language

## Description

Conventions, always-apply project memory, and `/tkmd-plan`, `/tkmd-save`, `/tkmd-do`, `/tkmd-shelf`, `/tkmd-plan-do`, and related skills must read the board writing language and write epic/story/task/bug markdown, static project README prose, and other agent-authored board markdown in that language. Chat language does not change the written language. If the field is missing, follow the init default (Cursor-agent usual language) and do not invent a second ad-hoc locale.

## Acceptance criteria

- [ ] `taskmark-conventions` and always-apply memory require all agent-written board markdown to use the stored writing language
- [ ] Plan, save, do, shelf, plan-do, and init skills instruct writing item titles, descriptions, user stories, acceptance criteria, and Prompt & feedback summaries in that language
- [ ] Plugin README states that chat language and board writing language are independent
- [ ] Skills do not translate existing committed markdown unless the current task is explicitly rewriting that file

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:29:52Z | prompt | Marco Mendão | `/tkmd-init` should let the user choose any project writing language (default: usual Cursor-agent language); work items, changelog, and README must always be written in that language even when chat is in another. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

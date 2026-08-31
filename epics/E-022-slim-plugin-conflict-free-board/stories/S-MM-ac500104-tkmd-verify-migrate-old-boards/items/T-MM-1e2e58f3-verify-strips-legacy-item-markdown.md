---
id: T-MM-1e2e58f3
type: task
title: Verify strips legacy fields and parent-only sections
status: backlog
priority: high
size: M
points: 5
parent: S-MM-ac500104
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, migration, markdown]
created: 2026-08-31
updated: 2026-08-31T12:22:27Z
started_at: null
completed_at: null
---

# T-MM-1e2e58f3: Verify strips legacy fields and parent-only sections

Scan `epics/**/*.md` and apply mechanical edits only. Strip retired frontmatter: `owner`, `estimate_minutes`, `estimate_source`, `estimate_basis`, `actual_minutes`, `actual_ms`, `size_source`, `size_basis`, `points_source`, `session_cap_minutes`. Keep spec keys, bodies, titles, acceptance criteria, and `in_progress` status. On `epic.md` and `story.md` only, remove child lists and parent Commits / Work log / Prompt & feedback sections. Do not strip those tables from task/bug leaves. Do not translate copy or rewrite IDs. Default is apply plus a summary; report-only when the user asks not to write yet.

## Acceptance criteria

- [ ] Listed retired frontmatter keys are removed from item files that still have them.
- [ ] Current spec keys, leaf Prompt & feedback, Commits, and Work log tables remain.
- [ ] Child lists and parent log sections are removed from `epic.md` and `story.md` only.
- [ ] Legacy sequential IDs and `in_progress` values are not rewritten.
- [ ] The command reports how many files were rewritten; it can skip writes when the user asks for a dry run.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T12:22:27Z | prompt | Marco Mendão | Cursor plan: `/tkmd-verify` migrates old boards to the current Taskmark layout and item spec. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

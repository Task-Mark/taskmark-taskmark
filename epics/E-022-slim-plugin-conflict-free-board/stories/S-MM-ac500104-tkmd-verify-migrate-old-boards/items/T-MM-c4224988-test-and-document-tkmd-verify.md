---
id: T-MM-c4224988
type: task
title: Test and document /tkmd-verify
status: backlog
priority: medium
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
tags: [plugin, tests, docs, website]
created: 2026-08-31
updated: 2026-08-31T12:22:27Z
started_at: null
completed_at: null
---

# T-MM-c4224988: Test and document /tkmd-verify

Cover `/tkmd-verify` with a fixture board that still has `INDEX.md`, retired frontmatter, and a `## Stories` section on an epic. After verify, forbidden files are gone, keys are gone, the parent section is gone, and the leaf work log remains. Document the command next to `/tkmd-init` on the website commands and setup pages: init is first create / light repair; verify migrates an existing board to the current layout.

## Acceptance criteria

- [ ] A plugin test (or fixture) fails if INDEX/SIZING/VELOCITY remain, retired keys remain, or a parent child-list section remains, and passes when a leaf Work log is kept.
- [ ] `/docs/commands` lists `/tkmd-verify` with a section on scaffold repair, deleting leftover generated files, and markdown cleanup.
- [ ] Setup (or workflows) states that `/tkmd-verify` never commits and that `/tkmd-commit` is still the only commit command.

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

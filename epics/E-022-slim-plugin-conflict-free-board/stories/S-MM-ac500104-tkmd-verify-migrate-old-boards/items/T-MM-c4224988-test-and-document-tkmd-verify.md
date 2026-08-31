---
id: T-MM-c4224988
type: task
title: Test and document /tkmd-verify
status: done
priority: medium
size: M
points: 5
parent: S-MM-ac500104
epic: E-022
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
tags: [plugin, tests, docs, website]
created: 2026-08-31
updated: 2026-08-31T13:06:14Z
started_at: 2026-08-31T13:01:00Z
completed_at: 2026-08-31T13:06:14Z
---

# T-MM-c4224988: Test and document /tkmd-verify

Cover `/tkmd-verify` with a fixture board that still has `INDEX.md`, retired frontmatter, and a `## Stories` section on an epic. After verify, forbidden files are gone, keys are gone, the parent section is gone, and the leaf work log remains. Document the command next to `/tkmd-init` on the website commands and setup pages: init is first create / light repair; verify migrates an existing board to the current layout.

## Acceptance criteria

- [x] A plugin test (or fixture) fails if INDEX/SIZING/VELOCITY remain, retired keys remain, or a parent child-list section remains, and passes when a leaf Work log is kept.
- [x] `/docs/commands` lists `/tkmd-verify` with a section on scaffold repair, deleting leftover generated files, and markdown cleanup.
- [x] Setup (or workflows) states that `/tkmd-verify` never commits and that `/tkmd-commit` is still the only commit command.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T12:22:27Z | prompt | Marco Mendão | Cursor plan: `/tkmd-verify` migrates old boards to the current Taskmark layout and item spec. |
| 2026-08-31T13:01:00Z | prompt | Marco Mendão | `/tkmd-do S-MM-ac500104`: implement `/tkmd-verify` to migrate old boards. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T13:01:00Z | 2026-08-31T13:02:08Z | Fixture tests and website docs for `/tkmd-verify` next to init. |

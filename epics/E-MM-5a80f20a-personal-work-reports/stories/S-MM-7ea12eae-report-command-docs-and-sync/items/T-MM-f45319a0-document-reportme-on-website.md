---
id: T-MM-f45319a0
type: task
title: Document /tkmd-reportme on the website
status: done
priority: medium
size: S
points: 3
parent: S-MM-7ea12eae
epic: E-MM-5a80f20a
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
tags: [docs, commands, website, reports]
created: 2026-08-31
updated: 2026-08-31T11:23:27Z
started_at: 2026-08-31T11:21:29Z
completed_at: 2026-08-31T11:23:27Z
---

# T-MM-f45319a0: Document /tkmd-reportme on the website

The Cursor plugin exposes `/tkmd-reportme`, but public docs still list only init, plan, save, plan-do, do, shelf, changelog, version, and commit. Add the command to the website command reference and to every page that enumerates the current slash set, matching the other `/tkmd-*` docs. Plugin READMEs already cover it.

## Acceptance criteria

- [x] `/docs/commands` lists `/tkmd-reportme` with purpose: report my done work since the last report into gitignored `.reports/`.
- [x] The commands page has a `/tkmd-reportme` section: board writing language, identity filter, never commits, never edits item markdown or `CHANGELOG.md`.
- [x] Docs overview, setup first-commands, and workflows mention `/tkmd-reportme` alongside the other slash commands.
- [x] Folder structure notes that `.reports/` is local-generated and gitignored like `REPOS.md`.
- [x] Docs still state that `/tkmd-commit` is the only command that commits.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T11:21:29Z | prompt | Marco Mendão | Check that every slash command in the system is documented on the website; add docs for any that are missing. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T11:21:29Z | 2026-08-31T11:23:27Z | Added /tkmd-reportme to website commands, setup, overview, workflows, and structure docs |

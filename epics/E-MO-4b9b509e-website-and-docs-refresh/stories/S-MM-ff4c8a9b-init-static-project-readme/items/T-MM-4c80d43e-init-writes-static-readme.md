---
id: T-MM-4c80d43e
type: task
title: Make /tkmd-init write a static project README
status: backlog
priority: high
size: M
points: 5
parent: S-MM-ff4c8a9b
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, init, readme]
created: 2026-08-29
updated: 2026-08-29T17:25:00Z
started_at: null
completed_at: null
---

# T-MM-4c80d43e: Make /tkmd-init write a static project README

## Description

Change `/tkmd-init` so it writes a static project README as part of board setup. Single-git: product-root `README.md` (not `taskmark/README.md`). Multi-git: workspace-level README beside the sibling product repos (not a generated board-root dashboard). Update the init command, `taskmark-init` skill, conventions, and always-apply memory: still forbid INDEX/SIZING/VELOCITY, README changelogs, Last synced, and `CHANGELOG.md` from init; allow this static README. Do not overwrite a richer existing README; create or repair only when missing or still a generated dashboard.

## Acceptance criteria

- [ ] `tkmd-init` command and `taskmark-init` skill instruct writing the static project README and no longer say “never create a board README” without distinguishing static project docs from dashboards
- [ ] Conventions and project-memory still forbid INDEX/SIZING/VELOCITY, generated README dashboards, and README changelogs; they allow the static project README from init
- [ ] Init does not write `CHANGELOG.md`, `INDEX.md`, `SIZING.md`, or `VELOCITY.md`
- [ ] Existing hand-written READMEs are not clobbered; missing or dashboard-style files are replaced with the static template

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:25:00Z | prompt | Marco Mendão | `/tkmd-init` should generate a static project README (purpose, system projects, local run, build, Vercel, Docker, `npx @taskmark/ui`). |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

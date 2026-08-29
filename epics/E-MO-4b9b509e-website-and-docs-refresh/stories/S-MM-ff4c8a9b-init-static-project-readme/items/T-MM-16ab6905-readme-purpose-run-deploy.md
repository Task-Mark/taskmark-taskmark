---
id: T-MM-16ab6905
type: task
title: Static README covers purpose, projects, run, and deploy
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
tags: [docs, readme, docker, vercel]
created: 2026-08-29
updated: 2026-08-29T17:25:00Z
started_at: null
completed_at: null
---

# T-MM-16ab6905: Static README covers purpose, projects, run, and deploy

## Description

Ship the init README template (and apply it on this Taskmark workspace if the current root README is thinner than the template). It must explain Taskmark’s purpose (conflict-resistant markdown product memory plus local board UI), list the git products in this system (board, Cursor plugin, frontend UI, website — or the discovered product roots for other workspaces), and give copy-paste instructions for local run, production build, Vercel, Docker, and standalone `npx @taskmark/ui`. Instructions must match current CLI behaviour (`npx taskmark serve` when installed locally; `npx @taskmark/ui` when there is no local install). Docker guidance must be runnable (add a board Dockerfile/compose stub if none exists). No Last synced, Current speed, open-work table, or README changelog.

## Acceptance criteria

- [ ] README explains Taskmark’s purpose in a short intro
- [ ] README lists the workspace product repositories (names and roles), not gitignored local absolute paths
- [ ] README documents local run (`npm install`, `npx taskmark serve` / `dev`, port 8275) and production `npm run build` / `out/`
- [ ] README documents Vercel using the board `vercel.json` static `out/` flow
- [ ] README documents Docker (image or compose that serves the board UI); stubs exist if the instructions need them
- [ ] README documents standalone `npx @taskmark/ui` (workspace/picker vs bound board) and does not tell users to `npx taskmark` without a local `@taskmark/ui` install
- [ ] No generated dashboard sections (Last synced, Current speed, open-work list, README changelog)

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:25:00Z | prompt | Marco Mendão | Static README from init: Taskmark purpose, system projects, local run, build, Vercel, Docker, and `npx @taskmark/ui`. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

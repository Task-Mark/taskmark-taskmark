---
id: T-242
type: task
title: Init always installs @taskmark/ui via npm
status: done
priority: high
size: M
size_source: suggested
size_basis: [calibrated:T-242]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_source: suggested
estimate_basis: [calibrated:T-242]
session_cap_minutes: 480
parent: S-052
epic: E-014
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
tags: [plugin, init, npm, ui]
created: 2026-07-28
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-28T14:30:38Z
completed_at: 2026-07-28T14:33:38Z
actual_ms: 180000
---
# T-242: Init always installs @taskmark/ui via npm

## Description

On first-time `taskmark-init`, scaffold a board `package.json` and run `npm install @taskmark/ui --save-dev` so `npx taskmark serve` works immediately. Re-running init on an existing board that lacks the UI package should install it (not only stop at “already initialized”).

## Acceptance criteria

- [x] `taskmark-init` writes board-ui stub `package.json` and `.gitignore` (`node_modules/`) on first init.
- [x] Init runs `npm install @taskmark/ui --save-dev` (fallback to local `@taskmark/ui` package path when registry 404 / unpublished).
- [x] Existing boards without UI install get the install step when the user asks to init / install UI.
- [x] Plugin synced to local install.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T14:30:38Z | prompt | Marco Mendão | taskmark-init must also npm-install @taskmark/ui on first init |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 3a3ef93 | taskmark-taskmark | 2026-07-28T14:35:04Z | Marco Mendão | log T-242 init ui install commits |
| fd924c0 | taskmark-cursor | 2026-07-28T14:34:41Z | Marco Mendão | install @taskmark/ui during taskmark-init |
| 082f140 | taskmark-taskmark | 2026-07-28T14:34:41Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T14:30:38Z | 2026-07-28T14:33:38Z | Init installs @taskmark/ui; board package.json + local file dep |

---
id: T-MM-89cb62e6
type: task
title: Persist writing language during /tkmd-init
status: done
priority: high
size: M
points: 5
parent: S-MM-9bcdb844
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
tags: [plugin, init, i18n]
created: 2026-08-29
updated: 2026-08-29T17:40:45Z
started_at: 2026-08-29T17:33:00Z
completed_at: 2026-08-29T17:40:45Z
---

# T-MM-89cb62e6: Persist writing language during /tkmd-init

## Description

Extend `/tkmd-init`, the `taskmark-init` skill, and board UI stub merge so a newly initialized or repaired board records a writing language. The user may choose any language. If they do not choose, use the language they usually use with the Cursor agent. Store it in a committed, merge-friendly board field (not INDEX/SIZING/VELOCITY/README). Existing boards missing the field get it on the next init/repair without clobbering other package.json keys.

## Acceptance criteria

- [x] `tkmd-init` command and `taskmark-init` skill ask for a writing language, allowing any language, with the Cursor-agent usual language as the default
- [x] Init/repair writes that language onto the board in a committed field that `ensure-board-ui.py` can merge
- [x] The field is documented in conventions; init still does not create INDEX, SIZING, VELOCITY, or `CHANGELOG.md`
- [x] Re-running init on an existing board keeps a previously stored language unless the user explicitly changes it

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:29:52Z | prompt | Marco Mendão | `/tkmd-init` should let the user choose any project writing language (default: usual Cursor-agent language); work items, changelog, and README must always be written in that language even when chat is in another. |
| 2026-08-29T17:33:00Z | prompt | Marco Mendão | `/tkmd-do S-MM-9bcdb844` |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T17:33:00Z | 2026-08-29T17:40:45Z | Persist `taskmark.writingLanguage` via init and `ensure-board-ui.py`. |

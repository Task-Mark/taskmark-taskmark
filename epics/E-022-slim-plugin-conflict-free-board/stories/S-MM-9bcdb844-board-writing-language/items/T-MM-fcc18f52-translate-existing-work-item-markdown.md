---
id: T-MM-fcc18f52
type: task
title: Translate existing work-item markdown into the board language
status: done
priority: high
size: XL
points: 13
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
tags: [board, i18n, markdown]
created: 2026-08-29
updated: 2026-08-29T17:40:45Z
started_at: 2026-08-29T17:33:00Z
completed_at: 2026-08-29T17:40:45Z
---

# T-MM-fcc18f52: Translate existing work-item markdown into the board language

## Description

After the board writing language is stored, rewrite human-readable prose on every existing epic, story, task, and bug so titles, descriptions, goals, user stories, acceptance/fix criteria, Prompt & feedback summaries, and work-log summaries use that language. Chat language does not apply. Keep IDs, paths, slugs, YAML keys, status values, sizes, dates, emails, SHAs, checkbox syntax, and table structure. Do not invent new items, change parent/epic links, or edit derived files. This is an explicit rewrite of existing leaves and parents; it is not the default for later `/tkmd-*` sessions.

## Acceptance criteria

- [x] Every `epic.md`, `story.md`, and task/bug leaf on this board has human-readable title and body text in the stored writing language
- [x] Frontmatter keys, IDs, `parent`/`epic`, status enums, sizing, tags-as-tokens, dates, reporter emails, commit SHAs, and file paths are unchanged
- [x] Prompt & feedback, Commits, and Work log tables keep their columns; only summary cells are translated
- [x] No INDEX/SIZING/VELOCITY/board dashboard README is created; parent files are edited only for this translation, not to add rollups or child lists

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:31:00Z | prompt | Marco Mendão | Translate all work items, changelog, and README to the writing language chosen for the Taskmark project. |
| 2026-08-29T17:33:00Z | prompt | Marco Mendão | `/tkmd-do S-MM-9bcdb844` |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T17:33:00Z | 2026-08-29T17:40:45Z | Translated remaining Portuguese work-item prose into English. |

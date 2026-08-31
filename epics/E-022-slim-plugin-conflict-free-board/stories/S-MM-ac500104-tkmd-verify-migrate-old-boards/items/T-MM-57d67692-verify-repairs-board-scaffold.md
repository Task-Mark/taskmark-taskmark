---
id: T-MM-57d67692
type: task
title: Verify repairs the board scaffold like init
status: done
priority: high
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
tags: [plugin, init, migration]
created: 2026-08-31
updated: 2026-08-31T13:06:14Z
started_at: 2026-08-31T13:01:00Z
completed_at: 2026-08-31T13:06:14Z
---

# T-MM-57d67692: Verify repairs the board scaffold like init

The verify skill locates the canonical board (single-git `taskmark/` vs sibling `*-taskmark`) via the same discovery as init/`sync-taskmark-repos.sh`. It keeps `taskmark.writingLanguage` unless missing. It runs `ensure-board-ui.py`, ensures gitignore includes `REPOS.md` and `.reports/`, installs `@taskmark/ui` as a production dependency, and repairs the static project README with init’s overwrite rules. Extra `taskmark/` trees in product repos are reported, not deleted, unless they are clearly generated duplicates.

## Acceptance criteria

- [x] Canonical board location matches init (single-git nested `taskmark/`, multi-git sibling board root).
- [x] `ensure-board-ui.py` is used; gitignore lists `REPOS.md` and `.reports/`; `@taskmark/ui` is a production dependency.
- [x] Static README is created or repaired only when missing, thinner than the template, or still a generated dashboard; single-git writes product-root README, not nested `taskmark/README.md`.
- [x] Missing writing language is filled; an existing stored language is kept.
- [x] Duplicate product-repo `taskmark/` copies are reported rather than silently deleted.

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
| Marco Mendão | 2026-08-31T13:01:00Z | 2026-08-31T13:02:08Z | Documented init-like scaffold repair and extra `taskmark/` reporting in the verify skill. |

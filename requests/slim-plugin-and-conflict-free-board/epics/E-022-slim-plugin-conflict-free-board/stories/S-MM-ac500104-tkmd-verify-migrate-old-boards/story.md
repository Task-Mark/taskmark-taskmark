---
id: S-MM-ac500104
type: story
title: Migrate old boards with /tkmd-verify
status: backlog
priority: high
size: null
points: null
parent: E-022
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, commands, migration, board]
created: 2026-08-31
updated: 2026-08-31T12:22:27Z
started_at: null
completed_at: null
---

# S-MM-ac500104: Migrate old boards with /tkmd-verify

## User story

As someone with a board created on an older Taskmark, I want `/tkmd-verify` to check the current layout rules, repair the scaffold the way `/tkmd-init` does, delete files that are no longer part of the product, and clean legacy fields from item markdown, so the board matches today’s conventions without a manual rewrite.

## Acceptance criteria

- [ ] The plugin exposes `/tkmd-verify`; it never commits or pushes and never creates `INDEX.md`, `SIZING.md`, `VELOCITY.md`, or `CHANGELOG.md`.
- [ ] It locates the canonical board, repairs UI stubs, gitignore (including `REPOS.md` and `.reports/`), `@taskmark/ui`, and the static project README using the same overwrite rules as init.
- [ ] At the canonical board root it deletes leftover generated files (`INDEX.md`, `SIZING.md`, `VELOCITY.md`, ID counter files) and a nested generated dashboard README when the static README is in the correct place.
- [ ] It strips retired frontmatter from item files and derived child-list/log sections from `epic.md` / `story.md` only, without translating bodies, rewriting IDs, or removing leaf Prompt & feedback, Commits, or Work log.
- [ ] Extra `taskmark/` copies in product repos are reported, not deleted, unless they are clearly generated duplicates of the canonical board.
- [ ] Plugin tests and website command docs cover the command next to `/tkmd-init`.

```mermaid
flowchart TD
  locate[Locate canonical board]
  scaffold[Repair scaffold like init]
  deleteGen[Delete forbidden generated files]
  migrateMd[Strip legacy frontmatter and parent sections]
  report[Report actions]
  locate --> scaffold --> deleteGen --> migrateMd --> report
```

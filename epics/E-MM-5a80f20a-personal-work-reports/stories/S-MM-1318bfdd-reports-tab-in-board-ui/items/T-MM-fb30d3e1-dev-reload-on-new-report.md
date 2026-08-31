---
id: T-MM-fb30d3e1
type: task
title: Reload the dev board when a report is written
status: done
priority: medium
size: XS
points: 1
parent: S-MM-1318bfdd
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
tags: [frontend, dev, reports]
created: 2026-08-31
updated: 2026-08-31T07:09:31Z
started_at: 2026-08-31T07:04:00Z
completed_at: 2026-08-31T07:09:31Z
---

# T-MM-fb30d3e1: Reload the dev board when a report is written

## Description

The markdown watcher used by `taskmark dev` skips every hidden directory, so files written under `.reports/` would never bump the polled mtime:

```js
function shouldIgnoreDir(name) {
  return IGNORE_DIRS.has(name) || name.startsWith(".")
}
```

Allow `.reports` through that check while keeping the other hidden and build directories ignored. The development reload route already descends into hidden directories, so it needs no change.

## Acceptance criteria

- [x] The board markdown watcher descends into `.reports/`
- [x] Writing or updating a report during `taskmark dev` triggers a reload
- [x] `node_modules`, `.git`, `out`, `.next`, `dist`, and `.taskmark-ui-build` stay ignored

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: reports live in a hidden `.reports` folder, which the dev watcher currently skips. |
| 2026-08-31T06:55:00Z | prompt | Marco Mendão | /tkmd-do E-MM-5a80f20a |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T07:04:00Z | 2026-08-31T07:06:00Z | Allowed the reports directory through the watcher's hidden-directory filter and confirmed a report write fires a reload. |

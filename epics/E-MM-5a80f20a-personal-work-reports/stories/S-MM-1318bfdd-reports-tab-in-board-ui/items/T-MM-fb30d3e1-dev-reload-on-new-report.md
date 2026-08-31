---
id: T-MM-fb30d3e1
type: task
title: Reload the dev board when a report is written
status: backlog
priority: medium
size: XS
points: 1
parent: S-MM-1318bfdd
epic: E-MM-5a80f20a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, dev, reports]
created: 2026-08-31
updated: 2026-08-31T06:47:12Z
started_at: null
completed_at: null
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

- [ ] The board markdown watcher descends into `.reports/`
- [ ] Writing or updating a report during `taskmark dev` triggers a reload
- [ ] `node_modules`, `.git`, `out`, `.next`, `dist`, and `.taskmark-ui-build` stay ignored

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: reports live in a hidden `.reports` folder, which the dev watcher currently skips. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|

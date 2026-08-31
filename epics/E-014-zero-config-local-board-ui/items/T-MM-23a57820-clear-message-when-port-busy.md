---
id: T-MM-23a57820
type: task
title: Report a clear message when the board port is already in use
status: done
priority: medium
size: XS
points: 1
parent: E-014
epic: E-014
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
tags: [cli, dev]
created: 2026-08-31
updated: 2026-08-31T18:16:30Z
started_at: 2026-08-31T17:54:03Z
completed_at: 2026-08-31T18:16:30Z
---

# T-MM-23a57820: Report a clear message when the board port is already in use

## Description

When another board (or a leftover process) already holds port 8275, `taskmark dev` and `taskmark serve` surface a raw Node stack:

```text
Error: listen EADDRINUSE: address already in use 0.0.0.0:8275
```

Check the port before spawning Next and exit with a short actionable message naming the port, the `--port` option, and how to find the process holding it. Do not silently fall back to another port: two boards answering on different ports would be more confusing than an explicit failure.

## Acceptance criteria

- [x] `taskmark dev` and `taskmark serve` detect a busy listen port before starting Next
- [x] The message names the busy port and suggests `--port` and how to identify the running process
- [x] No automatic fallback to a different port
- [x] A free port keeps the current behaviour with no extra output

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T17:50:00Z | prompt | Marco Mendão | From a Cursor plan: the reported terminal session also showed a raw EADDRINUSE stack on port 8275. |
| 2026-08-31T18:16:00Z | prompt | Marco Mendão | Confirm the work is finished and close the leaf. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T17:54:03Z | 2026-08-31T18:16:30Z | Pre-check listen port before Next; fail with `--port` and `lsof` guidance instead of EADDRINUSE. |

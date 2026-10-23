---
id: B-MM-4744c7c0
type: bug
title: Require Node.js runtimes patched for the October 2026 security release
status: done
priority: critical
size: S
points: 3
parent: E-MM-080acde6
epic: E-MM-080acde6
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
tags: [security, nodejs, docker, ci]
created: 2026-10-23
updated: 2026-10-23T15:08:26Z
started_at: 2026-10-23T15:02:47Z
completed_at: 2026-10-23T15:08:26Z
---
# B-MM-4744c7c0: Require Node.js runtimes patched for the October 2026 security release

## Description

Taskmark runtime declarations and container images allow Node.js versions affected by the October 21, 2026 security release, including high-severity DNS, TLS, and Brotli vulnerabilities.

## Fix criteria

- [x] Production and example container images use Node.js 22.23.4 or newer patched release lines.
- [x] Package engine declarations reject vulnerable and end-of-life Node.js release lines.
- [x] CI uses a patched Node.js version.
- [x] Relevant builds and checks pass on a patched runtime.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-10-23T15:02:47Z | prompt | Marco Mendão | Check the code against the Node.js October 2026 security release and fix any exposure found. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-10-23T15:02:47Z | 2026-10-23T15:08:26Z | Audited bulletin-specific API usage, pinned containers and CI to Node.js 22.23.4, constrained package engines to patched release lines, built the API image, and verified the runtime and engine range. |

---
id: E-MM-495d489d
type: epic
title: Cloud board markdown sync
status: backlog
priority: high
size: null
points: null
parent: null
epic: null
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, sync, api]
created: 2026-09-02
updated: 2026-09-02T17:54:46Z
started_at: null
completed_at: null
---
# E-MM-495d489d: Cloud board markdown sync

## Description

Push markdown boards from local Taskmark instances to Taskmark Cloud through the API, store files as the source of truth with a pre-built snapshot cache, and render a read-only hosted board that matches the local UI.

```mermaid
flowchart LR
  subgraph dev [Each developer machine]
    md[Board markdown files]
    cli["taskmark sync --watch"]
    md -->|mtime polling plus debounce| cli
  end
  subgraph api [taskmark-api NestJS plus Mongo]
    sync["PUT /v1/board-sync token identifies the project"]
    store[("ProjectSyncToken plus BoardFile plus BoardState")]
    readApi["GET snapshot and version"]
    sync --> store --> readApi
  end
  subgraph cloud [taskmark-cloud Next.js]
    bff[BFF proxy /api/v1]
    page["Board page using shared StaticBoardApp"]
    bff --> page
  end
  cli -->|"TASKMARK_SYNC_TOKEN env, hash diff"| sync
  readApi --> bff
  page -->|"poll version then refresh"| bff
  shared["@taskmark/components/board"]
  shared -.-> page
  shared -.->|"also used by the local board"| dev
```

## Goal

Developers share one project sync token, set it as `TASKMARK_SYNC_TOKEN` locally, and see their markdown board appear on Taskmark Cloud as a live read-only mirror.

## Acceptance criteria

- [ ] One opaque sync token per cloud project identifies the destination and authorizes local sync.
- [ ] Local instances send changed markdown files plus a BoardSnapshot cache whenever files change.
- [ ] The hosted board is read-only and reuses the same presentational board UI as the local app.
- [ ] Members can copy the token from project Settings; owners can rotate it.

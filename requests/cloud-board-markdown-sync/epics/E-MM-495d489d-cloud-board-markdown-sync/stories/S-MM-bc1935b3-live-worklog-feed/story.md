---
id: S-MM-bc1935b3
type: story
title: Live worklog feed across local and cloud boards
status: backlog
priority: high
size: null
points: null
parent: E-MM-495d489d
epic: E-MM-495d489d
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, sync, worklog, activity, ui]
created: 2026-09-03
updated: 2026-09-03T18:41:51Z
started_at: null
completed_at: null
---
# S-MM-bc1935b3: Live worklog feed across local and cloud boards

## Description

Surface team work-log activity as a floating Cloud feed and as a complete Worklog board view on both local and hosted boards. Reuse the existing markdown watcher and board-version refresh so activity and board content update automatically.

```mermaid
sequenceDiagram
  participant Agent as Agent_or_dev
  participant Md as Board_markdown
  participant Cli as taskmark_watch_sync
  participant Api as taskmark_api
  participant Cloud as Cloud_board_UI

  Agent->>Md: append Work log row
  Cli->>Md: mtime poll 750ms
  Cli->>Cli: rebuild snapshot extract leaf work logs
  Cli->>Api: PUT board-sync files snapshot activity
  Api->>Api: bump version store activity
  loop every 3s
    Cloud->>Api: GET boards activity
    Cloud->>Cloud: floating Messages max 6 TTL 5m
  end
  loop every 4s
    Cloud->>Api: GET boards version
    Cloud->>Cloud: refresh board and Worklog view
  end
```

## User story

As a team member, I can see which work teammates are recording now and browse the complete work-log history without opening every item.

## Acceptance criteria

- [ ] Cloud shows at most six floating work-log messages, removes each after five minutes, and evicts the oldest when full.
- [ ] Local and Cloud boards expose a Worklog view containing all leaf work-log rows.
- [ ] The local watcher sends new work-log activity through the existing authenticated sync flow.
- [ ] Cloud members can poll a compact activity endpoint.
- [ ] Full Cloud board content refreshes automatically after sync.

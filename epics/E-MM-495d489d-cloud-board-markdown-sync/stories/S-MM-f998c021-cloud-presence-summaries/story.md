---
id: S-MM-f998c021
type: story
title: Cloud presence summaries from recent worklogs
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
tags: [cloud, worklog, presence, ai]
created: 2026-09-03
updated: 2026-09-03T21:56:00Z
started_at: null
completed_at: null
---
# S-MM-f998c021: Cloud presence summaries from recent worklogs

## Description

Show who is working now on the Cloud board. Keep the left speedometer. On the right, keep the last five worklog bubbles and stack presence cards above them in the same message chrome: one card per person, a quoted present-tense sentence, no item code tag. A later pulse replaces that person's card.

The API lazily summarizes each person's new worklogs every 30 minutes when a member polls activity, so multiple Cloud tabs do not each call the model.

```mermaid
sequenceDiagram
  participant Sync as board_sync
  participant Api as taskmark_api
  participant Llm as OpenAI_compatible
  participant Cloud as Cloud_UI

  Sync->>Api: PUT board-sync with worklog events
  Api->>Api: merge recentActivity
  loop poll 3s
    Cloud->>Api: GET activity
    Api->>Api: if 30m elapsed and new events per actor
    Api->>Llm: summarize that actor window
    Api-->>Cloud: recent plus presence
    Cloud->>Cloud: replace that actor card
  end
```

## User story

As a Cloud teammate looking at the board, I want a short “what they are doing now” sentence for each person who recently logged work so I can see current focus without reading every worklog.

## Acceptance criteria

- [ ] Cloud shows presence cards above the floating worklog feed, one card per person, replacing that person on later pulses.
- [ ] Presence is not mixed into stored recent activity and is not shown on the local board.
- [ ] The API refreshes presence at most every 30 minutes, only for actors with new worklogs since the last tick.
- [ ] Cards older than two hours drop off. The sentence is English present tense; without an LLM key the API still returns an extractive fallback.

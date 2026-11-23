---
id: S-MM-8b9dffc8
type: story
title: Explain Taskmark Cloud on the public website
status: backlog
priority: high
size: null
points: null
parent: E-MO-4b9b509e
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [website, docs, cloud]
created: 2026-09-15
updated: 2026-09-15T16:37:00Z
started_at: null
completed_at: null
---
# S-MM-8b9dffc8: Explain Taskmark Cloud on the public website

## Description

Add public website copy for Taskmark Cloud: why the hosted board exists, and how a local markdown board publishes to it. Keep the local plugin as the source of truth; Cloud is the shared, read-mostly team view.

## User story

As a visitor, I want the website to explain Taskmark Cloud and how my local board syncs to it so I know why to open cloud.taskmark.dev and how to connect a project.

## Acceptance criteria

- [ ] The marketing landing page has a Cloud section that states the purpose of Taskmark Cloud.
- [ ] Docs include a Cloud page that walks through connecting a local board via the committed `.config` token.
- [ ] Navigation reaches the Cloud docs from the site header, footer, and docs sidebar.
- [ ] Copy matches current product behaviour: token from Cloud Settings, token in board `.config`, `taskmark dev` / `taskmark serve` push markdown.

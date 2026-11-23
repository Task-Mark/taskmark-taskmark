---
id: R-cloud-authentication-and-registration
type: request
title: Cloud authentication and registration
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-09-02
updated: 2026-09-02T15:28:10Z
forecast: null
tags:
  - cloud
  - api
  - auth
aliases:
  - E-MM-63bde04a
source_meetings: []
links: []
---

# Cloud authentication and registration

## Goal

A person can register, verify email, sign in with secure cookies, name a first project, and invite others by email without exposing credentials or enumerating accounts.

## Done when

- [ ] Registration creates a pending user and pending project and does not start a session.
- [ ] Email verification activates the owner membership and then sends invitations.
- [ ] Login issues rotating HttpOnly access and refresh cookies.
- [ ] Invitations work for both existing and unknown emails.
- [ ] Secrets stay in local env files; no live credentials are committed.

## Out of scope

_Nothing yet._

## Open questions

_None yet._

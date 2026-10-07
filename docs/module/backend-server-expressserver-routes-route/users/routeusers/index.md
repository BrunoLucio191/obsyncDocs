---
title: RouteUsers
kind: class
longname: module:backend/Server/ExpressServer/routes/route.users.RouteUsers
description: "User management endpoints, mounted at /api/users in ExpressServer. Full paths: GET /api/users auth, admin POST /api/users auth, admin, clientId PATCH /api/users/:id/name auth, admin, clientId PATCH /api/users/:id/password auth, admin, clientId PATCH /api/users/:id/role auth, admin, clientId PATCH /api/users/:id/status auth, admin, clientId DELETE /api/users/:id auth, admin, clientId"
---

# RouteUsers

<SourceLink href="/source/backend/server/expressserver/routes/route-users-ts/#L23" label="route.users.ts:23" />

User management endpoints, mounted at `/api/users` in ExpressServer.

Full paths:

- GET /api/users auth, admin
- POST /api/users auth, admin, clientId
- PATCH /api/users/:id/name auth, admin, clientId
- PATCH /api/users/:id/password auth, admin, clientId
- PATCH /api/users/:id/role auth, admin, clientId
- PATCH /api/users/:id/status auth, admin, clientId
- DELETE /api/users/:id auth, admin, clientId

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new RouteUsers(
	__namedParameters: RouteUsersContructor,
): RouteUsers"
/>

**Parameters**

- `__namedParameters` (RouteUsersContructor)

**Returns**

`RouteUsers`

---

## Properties

<MemberHeading id="router" depth="3" name="router" sig="router: Router" />

<MemberMeta sourceHref="/source/backend/server/expressserver/routes/route-users-ts/#L24" sourceLabel="route.users.ts:24" />

## Methods

<MemberHeading id="startroute" depth="3" name="startRoute" sig="startRoute(): void" />

<MemberMeta sourceHref="/source/backend/server/expressserver/routes/route-users-ts/#L41" sourceLabel="route.users.ts:41" />

**Returns**

- `void`

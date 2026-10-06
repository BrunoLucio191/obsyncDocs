---
title: RouteSyncFiles
kind: class
longname: RouteSyncFiles
description: "Vault sync endpoints, mounted at /api/sync in ExpressServer. Full paths: POST /api/sync/initSync auth, clientId POST /api/sync/create auth, admin, clientId DELETE /api/sync/delete auth, admin, clientId PUT /api/sync/modify auth, admin, clientId PUT /api/sync/rename auth, admin, clientId POST /api/sync/createFile auth, admin, clientId (raw body) GET /api/sync/getFile?path&#x26;fileName auth, clientId"
---

# RouteSyncFiles

<SourceLink href="/source/backend/server/expressserver/routes/route-syncfiles-ts/#L28" label="route.syncFiles.ts:28" />

Vault sync endpoints, mounted at `/api/sync` in ExpressServer.

Full paths:

- POST /api/sync/initSync auth, clientId
- POST /api/sync/create auth, admin, clientId
- DELETE /api/sync/delete auth, admin, clientId
- PUT /api/sync/modify auth, admin, clientId
- PUT /api/sync/rename auth, admin, clientId
- POST /api/sync/createFile auth, admin, clientId (raw body)
- GET /api/sync/getFile?path\&fileName auth, clientId

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new RouteSyncFiles(
	__namedParameters: RouteSyncFilesContructor,
): RouteSyncFiles"
/>

**Parameters**

- `__namedParameters` ([RouteSyncFilesContructor](/routesyncfilescontructor))

**Returns**

`RouteSyncFiles`

---

## Properties

<MemberHeading id="router" depth="3" name="router" sig="router: Router" />

<MemberMeta sourceHref="/source/backend/server/expressserver/routes/route-syncfiles-ts/#L29" sourceLabel="route.syncFiles.ts:29" />

## Methods

<MemberHeading id="startroute" depth="3" name="startRoute" sig="startRoute(): void" />

<MemberMeta sourceHref="/source/backend/server/expressserver/routes/route-syncfiles-ts/#L58" sourceLabel="route.syncFiles.ts:58" />

**Returns**

- `void`

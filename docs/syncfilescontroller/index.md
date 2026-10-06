---
title: SyncFilesController
kind: class
longname: SyncFilesController
description: Orquestrate files/directories modifications done via http routes as a single object that is called by {@link RouteSyncFiles}
---

# SyncFilesController

<SourceLink href="/source/backend/server/expressserver/controllers/syncfilescontroller-ts/#L24" label="SyncFilesController.ts:24" />

Orquestrate files/directories modifications done via http routes as a single object that is called by [RouteSyncFiles](/routesyncfiles)

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new SyncFilesController(
	__namedParameters: SyncFilesControllerConstructor,
): SyncFilesController"
/>

**Parameters**

- `__namedParameters` ([SyncFilesControllerConstructor](/syncfilescontrollerconstructor))

**Returns**

`SyncFilesController`

---

## Methods

<MemberHeading id="create" depth="3" name="create" sig="create(req: Request, res: Response): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/expressserver/controllers/syncfilescontroller-ts/#L98" sourceLabel="SyncFilesController.ts:98" />

Crestes files or directories in the canonical Vault, also modifies the YjsPersistence

**Parameters**

- `req` (Request)
- `res` (Response)

**Returns**

- `Promise<void>`

<MemberHeading id="createfile" depth="3" name="createFile" sig="createFile(req: Request, res: Response): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/expressserver/controllers/syncfilescontroller-ts/#L279" sourceLabel="SyncFilesController.ts:279" />

Expects the raw body already parsed by `express.raw` in the route.

**Parameters**

- `req` (Request)
- `res` (Response)

**Returns**

- `Promise<void>`

<MemberHeading id="delete" depth="3" name="delete" sig="delete(req: Request, res: Response): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/expressserver/controllers/syncfilescontroller-ts/#L148" sourceLabel="SyncFilesController.ts:148" />

**Parameters**

- `req` (Request)
- `res` (Response)

**Returns**

- `Promise<void>`

<MemberHeading id="getfile" depth="3" name="getFile" sig="getFile(req: Request, res: Response): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/expressserver/controllers/syncfilescontroller-ts/#L316" sourceLabel="SyncFilesController.ts:316" />

**Parameters**

- `req` (Request)
- `res` (Response)

**Returns**

- `Promise<void>`

<MemberHeading id="initsync" depth="3" name="initSync" sig="initSync(req: Request, res: Response): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/expressserver/controllers/syncfilescontroller-ts/#L59" sourceLabel="SyncFilesController.ts:59" />

Responsible for doing the inital sync on the whole vault, download all the missing changes while offline 204 when the client's `X-ObSync-Gene` matches the current gene, otherwise the zip with the current gene.

**Parameters**

- `req` (Request)
- `res` (Response)

**Returns**

- `Promise<void>`

<MemberHeading id="modify" depth="3" name="modify" sig="modify(req: Request, res: Response): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/expressserver/controllers/syncfilescontroller-ts/#L183" sourceLabel="SyncFilesController.ts:183" />

**Parameters**

- `req` (Request)
- `res` (Response)

**Returns**

- `Promise<void>`

<MemberHeading id="rename" depth="3" name="rename" sig="rename(req: Request, res: Response): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/expressserver/controllers/syncfilescontroller-ts/#L217" sourceLabel="SyncFilesController.ts:217" />

Route responsible for dealing with all the renames

**Parameters**

- `req` (Request)
- `res` (Response)

**Returns**

- `Promise<void>`

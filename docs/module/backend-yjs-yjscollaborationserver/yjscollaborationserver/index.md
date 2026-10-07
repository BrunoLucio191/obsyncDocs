---
title: YjsCollaborationServer
kind: class
longname: module:backend/yjs/YjsCollaborationServer.YjsCollaborationServer
description: Entry point of the Yjs backend for the rest of the server.
---

# YjsCollaborationServer

<SourceLink href="/source/backend/yjs/yjscollaborationserver-ts/#L22" label="YjsCollaborationServer.ts:22" />

Entry point of the Yjs backend for the rest of the server.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new YjsCollaborationServer(): YjsCollaborationServer" />

**Returns**

`YjsCollaborationServer`

---

## Methods

<MemberHeading id="clearpathdeleted" depth="3" name="clearPathDeleted" sig="clearPathDeleted(targetPath: string): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L45" sourceLabel="YjsCollaborationServer.ts:45" />

**Parameters**

- `targetPath` (string)

**Returns**

- `void`

<MemberHeading id="deletepersistedstateunderpath" depth="3" name="deletePersistedStateUnderPath" sig="deletePersistedStateUnderPath(targetPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L49" sourceLabel="YjsCollaborationServer.ts:49" />

**Parameters**

- `targetPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="isdocumentinvalidated" depth="3" name="isDocumentInvalidated" sig="isDocumentInvalidated(doc: Doc): boolean" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L36" sourceLabel="YjsCollaborationServer.ts:36" />

**Parameters**

- `doc` (Doc)

**Returns**

- `boolean`

<MemberHeading id="ispathdeleted" depth="3" name="isPathDeleted" sig="isPathDeleted(filePath: string): boolean" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L32" sourceLabel="YjsCollaborationServer.ts:32" />

**Parameters**

- `filePath` (string)

**Returns**

- `boolean`

<MemberHeading id="markpathdeleted" depth="3" name="markPathDeleted" sig="markPathDeleted(targetPath: string): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L40" sourceLabel="YjsCollaborationServer.ts:40" />

**Parameters**

- `targetPath` (string)

**Returns**

- `void`

<MemberHeading
  id="renamepersistedstatepath"
  depth="3"
  name="renamePersistedStatePath"
  sig="renamePersistedStatePath(
	oldPath: string,
	newPath: string,
): Promise<void>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L57" sourceLabel="YjsCollaborationServer.ts:57" />

**Parameters**

- `oldPath` (string)
- `newPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="setpersistence" depth="3" name="setPersistence" sig="setPersistence(adapter: YjsPersistenceAdapter): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L28" sourceLabel="YjsCollaborationServer.ts:28" />

**Parameters**

- `adapter` ([YjsPersistenceAdapter](/module/backend-yjs-yjs/types/yjspersistenceadapter))

**Returns**

- `void`

<MemberHeading
  id="setupconnection"
  depth="3"
  name="setupConnection"
  sig="setupConnection(
	connection: WebSocket,
	request: IncomingMessage,
	authenticatedUser: YjsAuthenticatedConnection,
): Promise<YjsRoom>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L67" sourceLabel="YjsCollaborationServer.ts:67" />

**Parameters**

- `connection` (WebSocket)
- `request` (IncomingMessage)
- `authenticatedUser` ([YjsAuthenticatedConnection](/module/backend-yjs-yjs/types/yjsauthenticatedconnection))

**Returns**

- `Promise<`[`YjsRoom`](/module/backend-yjs-yjsrooms-yjsroom/yjsroom)`>`

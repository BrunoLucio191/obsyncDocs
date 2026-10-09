---
title: YjsCollaborationServer
kind: class
longname: module:backend/yjs/YjsCollaborationServer.YjsCollaborationServer
description: Entry point of the Yjs backend for the rest of the server.
---

# YjsCollaborationServer

<SourceLink href="/source/backend/yjs/yjscollaborationserver-ts/#L24" label="YjsCollaborationServer.ts:24" />

Entry point of the Yjs backend for the rest of the server.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new YjsCollaborationServer(): YjsCollaborationServer" />

**Returns**

`YjsCollaborationServer`

---

## Methods

<MemberHeading id="clearpathdeleted" depth="3" name="clearPathDeleted" sig="clearPathDeleted(targetPath: string): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L48" sourceLabel="YjsCollaborationServer.ts:48" />

**Parameters**

- `targetPath` (string)

**Returns**

- `void`

<MemberHeading id="deletepersistedstateunderpath" depth="3" name="deletePersistedStateUnderPath" sig="deletePersistedStateUnderPath(targetPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L52" sourceLabel="YjsCollaborationServer.ts:52" />

**Parameters**

- `targetPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="isdocumentinvalidated" depth="3" name="isDocumentInvalidated" sig="isDocumentInvalidated(doc: Doc): boolean" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L39" sourceLabel="YjsCollaborationServer.ts:39" />

**Parameters**

- `doc` (Doc)

**Returns**

- `boolean`

<MemberHeading id="ispathdeleted" depth="3" name="isPathDeleted" sig="isPathDeleted(filePath: string): boolean" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L35" sourceLabel="YjsCollaborationServer.ts:35" />

**Parameters**

- `filePath` (string)

**Returns**

- `boolean`

<MemberHeading id="markpathdeleted" depth="3" name="markPathDeleted" sig="markPathDeleted(targetPath: string): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L43" sourceLabel="YjsCollaborationServer.ts:43" />

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

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L60" sourceLabel="YjsCollaborationServer.ts:60" />

**Parameters**

- `oldPath` (string)
- `newPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="setpersistence" depth="3" name="setPersistence" sig="setPersistence(adapter: YjsPersistenceAdapter): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L31" sourceLabel="YjsCollaborationServer.ts:31" />

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

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjscollaborationserver-ts/#L70" sourceLabel="YjsCollaborationServer.ts:70" />

**Parameters**

- `connection` (WebSocket)
- `request` (IncomingMessage)
- `authenticatedUser` ([YjsAuthenticatedConnection](/module/backend-yjs-yjs/types/yjsauthenticatedconnection))

**Returns**

- `Promise<`[`YjsRoom`](/module/backend-yjs-yjsrooms-yjsroom/yjsroom)`>`

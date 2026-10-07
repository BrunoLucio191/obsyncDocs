---
title: YjsRoom
kind: class
longname: module:backend/yjs/yjsRooms/YjsRoom.YjsRoom
description: One collaborative document, its awareness and its connections. Lifecycle lives in YjsRoomRegistry.
---

# YjsRoom

<SourceLink href="/source/backend/yjs/yjsrooms/yjsroom-ts/#L11" label="YjsRoom.ts:11" />

One collaborative document, its awareness and its connections. Lifecycle lives in YjsRoomRegistry.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new YjsRoom(docName: string, filePath: string): YjsRoom" />

**Parameters**

- `docName` (string)
- `filePath` (string)

**Returns**

`YjsRoom`

---

## Properties

<MemberHeading id="awareness" depth="3" name="awareness" sig="awareness: Awareness" />

<MemberMeta badges="readonly" sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L15" sourceLabel="YjsRoom.ts:15" />

<MemberHeading id="awarenessowners" depth="3" name="awarenessOwners" sig="awarenessOwners: Map<number, WebSocket>" />

<MemberMeta badges="readonly" sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L17" sourceLabel="YjsRoom.ts:17" />

<MemberHeading id="closingpromise" depth="3" name="closingPromise" sig="closingPromise: Promise<void>" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L22" sourceLabel="YjsRoom.ts:22" />

**Default:** `null`

<MemberHeading id="connections" depth="3" name="connections" sig="connections: Map<WebSocket, YjsConnectionState>" />

<MemberMeta badges="readonly" sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L16" sourceLabel="YjsRoom.ts:16" />

<MemberHeading id="doc" depth="3" name="doc" sig="doc: Doc" />

<MemberMeta badges="readonly" sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L14" sourceLabel="YjsRoom.ts:14" />

<MemberHeading id="docname" depth="3" name="docName" sig="docName: string" />

<MemberMeta badges="readonly" sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L12" sourceLabel="YjsRoom.ts:12" />

<MemberHeading id="filepath" depth="3" name="filePath" sig="filePath: string" />

<MemberMeta badges="readonly" sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L13" sourceLabel="YjsRoom.ts:13" />

<MemberHeading id="messagequeue" depth="3" name="messageQueue" sig="messageQueue: Promise<void>" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L19" sourceLabel="YjsRoom.ts:19" />

<MemberHeading id="pendingmessages" depth="3" name="pendingMessages" sig="pendingMessages: number" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L20" sourceLabel="YjsRoom.ts:20" />

**Default:** `0`

<MemberHeading id="ready" depth="3" name="ready" sig="ready: Promise<void>" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L18" sourceLabel="YjsRoom.ts:18" />

<MemberHeading id="reservations" depth="3" name="reservations" sig="reservations: number" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L21" sourceLabel="YjsRoom.ts:21" />

**Default:** `1`

## Methods

<MemberHeading id="attachlisteners" depth="3" name="attachListeners" sig="attachListeners(isInvalidated: () => boolean): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L33" sourceLabel="YjsRoom.ts:33" />

`isInvalidated` stops broadcasts of a document deleted while the room was loading.

**Parameters**

- `isInvalidated` (() => boolean)

**Returns**

- `void`

<MemberHeading id="broadcast" depth="3" name="broadcast" sig="broadcast(message: Uint8Array): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L74" sourceLabel="YjsRoom.ts:74" />

**Parameters**

- `message` (Uint8Array)

**Returns**

- `void`

<MemberHeading id="destroydocument" depth="3" name="destroyDocument" sig="destroyDocument(): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L128" sourceLabel="YjsRoom.ts:128" />

**Returns**

- `void`

<MemberHeading id="releaseconnection" depth="3" name="releaseConnection" sig="releaseConnection(connection: WebSocket): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L102" sourceLabel="YjsRoom.ts:102" />

**Parameters**

- `connection` (WebSocket)

**Returns**

- `void`

<MemberHeading id="sendawarenesssnapshot" depth="3" name="sendAwarenessSnapshot" sig="sendAwarenessSnapshot(connection: WebSocket): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L80" sourceLabel="YjsRoom.ts:80" />

**Parameters**

- `connection` (WebSocket)

**Returns**

- `void`

<MemberHeading id="sendinitialsync" depth="3" name="sendInitialSync" sig="sendInitialSync(connection: WebSocket): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroom-ts/#L93" sourceLabel="YjsRoom.ts:93" />

**Parameters**

- `connection` (WebSocket)

**Returns**

- `void`

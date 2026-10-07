---
title: YjsRoomRegistry
kind: class
longname: module:backend/yjs/yjsRooms/YjsRoomRegistry.YjsRoomRegistry
description: A room lives while it has connections or reservations, then is flushed and destroyed.
---

# YjsRoomRegistry

<SourceLink href="/source/backend/yjs/yjsrooms/yjsroomregistry-ts/#L9" label="YjsRoomRegistry.ts:9" />

A room lives while it has connections or reservations, then is flushed and destroyed.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new YjsRoomRegistry(
	deletedPaths: DeletedPathRegistry,
	persistence: YjsPersistenceGateway,
): YjsRoomRegistry"
/>

**Parameters**

- `deletedPaths` ([DeletedPathRegistry](/module/backend-yjs-deletedpathregistry/deletedpathregistry))
- `persistence` ([YjsPersistenceGateway](/module/backend-yjs-yjspersistencegateway/yjspersistencegateway))

**Returns**

`YjsRoomRegistry`

---

## Methods

<MemberHeading id="invalidateunderpath" depth="3" name="invalidateUnderPath" sig="invalidateUnderPath(targetPath: string): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroomregistry-ts/#L41" sourceLabel="YjsRoomRegistry.ts:41" />

**Parameters**

- `targetPath` (string)

**Returns**

- `void`

<MemberHeading id="release" depth="3" name="release" sig="release(room: YjsRoom, connection: WebSocket): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroomregistry-ts/#L36" sourceLabel="YjsRoomRegistry.ts:36" />

**Parameters**

- `room` ([YjsRoom](/module/backend-yjs-yjsrooms-yjsroom/yjsroom))
- `connection` (WebSocket)

**Returns**

- `void`

<MemberHeading id="reserve" depth="3" name="reserve" sig="reserve(docName: string, filePath: string): YjsRoom" />

<MemberMeta sourceHref="/source/backend/yjs/yjsrooms/yjsroomregistry-ts/#L23" sourceLabel="YjsRoomRegistry.ts:23" />

The reservation keeps the room alive until the caller attaches its connection.

**Parameters**

- `docName` (string)
- `filePath` (string)

**Returns**

- [`YjsRoom`](/module/backend-yjs-yjsrooms-yjsroom/yjsroom)

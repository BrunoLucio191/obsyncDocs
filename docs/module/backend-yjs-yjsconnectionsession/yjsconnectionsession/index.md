---
title: YjsConnectionSession
kind: class
longname: module:backend/yjs/YjsConnectionSession.YjsConnectionSession
---

# YjsConnectionSession

<SourceLink href="/source/backend/yjs/yjsconnectionsession-ts/#L24" label="YjsConnectionSession.ts:24" />

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new YjsConnectionSession(
	room: YjsRoom,
	connection: WebSocket,
	connectionState: YjsConnectionState,
	deletedPaths: DeletedPathRegistry,
	syncHandler: SyncMessageHandlerFn,
	messageCounter: WebSocketMessageCounter<WebSocket, number>,
): YjsConnectionSession"
/>

**Parameters**

- `room` ([YjsRoom](/module/backend-yjs-yjsrooms-yjsroom/yjsroom))
- `connection` (WebSocket)
- `connectionState` ([YjsConnectionState](/module/backend-yjs-yjs/types/yjsconnectionstate))
- `deletedPaths` ([DeletedPathRegistry](/module/backend-yjs-deletedpathregistry/deletedpathregistry))
- `syncHandler` ([SyncMessageHandlerFn](/module/backend-yjs-syncmessagehandler/syncmessagehandlerfn))
- `messageCounter` ([WebSocketMessageCounter](/module/backend-yjs-yjsutils-messagecounter/utils/websocketmessagecounter)\<WebSocket, number>)

**Returns**

`YjsConnectionSession`

---

## Methods

<MemberHeading id="handlerawmessage" depth="3" name="handleRawMessage" sig="handleRawMessage(rawData: RawData, isBinary: boolean): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsconnectionsession-ts/#L52" sourceLabel="YjsConnectionSession.ts:52" />

Receives the raw message and adds that to the queue

**Parameters**

- `rawData` (RawData)
- `isBinary` (boolean) — if the data received is not binary, the connection is closed

**Returns**

- `void`

---
title: YjsConnectionSession
kind: class
longname: YjsConnectionSession
---

# YjsConnectionSession

<SourceLink href="/source/backend/yjs/yjsconnectionsession-ts/#L23" label="YjsConnectionSession.ts:23" />

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
): YjsConnectionSession"
/>

**Parameters**

- `room` ([YjsRoom](/yjsroom))
- `connection` (WebSocket)
- `connectionState` ([YjsConnectionState](/yjsconnectionstate))
- `deletedPaths` ([DeletedPathRegistry](/deletedpathregistry))
- `syncHandler` ([SyncMessageHandlerFn](/syncmessagehandlerfn))

**Returns**

`YjsConnectionSession`

---

## Methods

<MemberHeading id="handlerawmessage" depth="3" name="handleRawMessage" sig="handleRawMessage(rawData: RawData, isBinary: boolean): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsconnectionsession-ts/#L44" sourceLabel="YjsConnectionSession.ts:44" />

**Parameters**

- `rawData` (RawData)
- `isBinary` (boolean)

**Returns**

- `void`

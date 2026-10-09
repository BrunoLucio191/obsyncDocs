---
title: closeConnection
kind: function
longname: module:backend/yjs/yjsUtils/wsTransport.utils.closeConnection
description: The reason is cut to the protocol's 123-byte limit.
---

# closeConnection

<Signature
  code="closeConnection(
	connection: WebSocket,
	code: number,
	reason: string,
): void"
/>

<SourceLink href="/source/backend/yjs/yjsutils/wstransport-utils-ts/#L36" label="wsTransport.utils.ts:36" />

The reason is cut to the protocol's 123-byte limit.

**Parameters**

- `connection` (WebSocket)
- `code` (number)
- `reason` (string)

**Returns**

- `void`

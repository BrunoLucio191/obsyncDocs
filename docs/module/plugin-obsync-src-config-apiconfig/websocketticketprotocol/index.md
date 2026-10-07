---
title: webSocketTicketProtocol
kind: function
longname: module:plugin/obSync/src/config/ApiConfig.webSocketTicketProtocol
description: The ticket goes in the subprotocol because a WebSocket upgrade can't carry an Authorization header.
---

# webSocketTicketProtocol

<Signature code="webSocketTicketProtocol(ticket: string): string" />

<SourceLink href="/source/plugin/obsync/src/config/apiconfig-ts/#L32" label="ApiConfig.ts:32" />

The ticket goes in the subprotocol because a WebSocket upgrade can't carry an `Authorization` header.

**Parameters**

- `ticket` (string)

**Returns**

- `string`

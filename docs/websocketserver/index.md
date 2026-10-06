---
title: WebSocketServer
kind: class
longname: WebSocketServer
description: /system (receive-only vault change broadcasts) and /yjs (collaboration), both authenticated by ticket. Connections close when their session is revoked or the user's authorization changes.
---

# WebSocketServer

<SourceLink href="/source/backend/server/websocketserver-ts/#L20" label="WebSocketServer.ts:20" />

`/system` (receive-only vault change broadcasts) and `/yjs` (collaboration), both authenticated by ticket. Connections close when their session is revoked or the user's authorization changes.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new WebSocketServer(
	server: Server,
	tokenService: TokenService,
	requireTls: boolean,
	trustProxy: boolean,
	collaborationServer: YjsCollaborationServer,
): WebSocketServer"
/>

**Parameters**

- `server` (Server)
- `tokenService` ([TokenService](/tokenservice))
- `requireTls` (boolean)
- `trustProxy` (boolean)
- `collaborationServer` ([YjsCollaborationServer](/yjscollaborationserver))

**Returns**

`WebSocketServer`

---

## Properties

<MemberHeading id="wsssystem" depth="3" name="wssSystem" sig="wssSystem: WebSocketServer" />

<MemberMeta badges="readonly" sourceHref="/source/backend/server/websocketserver-ts/#L21" sourceLabel="WebSocketServer.ts:21" />

<MemberHeading id="wssyjs" depth="3" name="wssYjs" sig="wssYjs: WebSocketServer" />

<MemberMeta badges="readonly" sourceHref="/source/backend/server/websocketserver-ts/#L22" sourceLabel="WebSocketServer.ts:22" />

## Methods

<MemberHeading id="initializewebsockets" depth="3" name="initializeWebSockets" sig="initializeWebSockets(): void" />

<MemberMeta sourceHref="/source/backend/server/websocketserver-ts/#L137" sourceLabel="WebSocketServer.ts:137" />

Call once, before the server takes traffic. A `/system` client that sends anything is closed.

**Returns**

- `void`

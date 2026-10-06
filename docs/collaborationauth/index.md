---
title: CollaborationAuth
kind: interface
longname: CollaborationAuth
---

# CollaborationAuth

<Signature
  code="interface CollaborationAuth {
	user: AuthenticatedUser;
	createWebSocketTicket(channel: 'yjs'): Promise<string>;
	isReadOnlyUser(): boolean;
}"
/>

<SourceLink href="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L8" label="CollaborationController.ts:8" />

---

## Properties

<MemberHeading id="user" depth="3" name="user" sig="user: AuthenticatedUser" />

<MemberMeta badges="readonly" sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L9" sourceLabel="CollaborationController.ts:9" />

## Methods

<MemberHeading id="createwebsocketticket" depth="3" name="createWebSocketTicket" sig="createWebSocketTicket(channel: 'yjs'): Promise<string>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L11" sourceLabel="CollaborationController.ts:11" />

**Parameters**

- `channel` ("yjs")

**Returns**

- `Promise<string>`

<MemberHeading id="isreadonlyuser" depth="3" name="isReadOnlyUser" sig="isReadOnlyUser(): boolean" />

<MemberMeta sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L10" sourceLabel="CollaborationController.ts:10" />

**Returns**

- `boolean`

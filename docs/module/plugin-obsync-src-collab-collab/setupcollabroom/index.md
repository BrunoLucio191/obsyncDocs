---
title: setupCollabRoom
kind: function
longname: module:plugin/obSync/src/collab/collab.setupCollabRoom
description: "Doesn't connect yet: call connect() once the editor still shows this file. Regular users edit a private doc that only receives network updates, so nothing leaks upstream."
---

# setupCollabRoom

<Signature
  code="setupCollabRoom(
	fileName: string,
	user: CollaborationUser,
	requestWebSocketTicket: () => Promise<string>,
	onUserJoined: (name: string) => void,
	onUserLeft: (name: string) => void,
): Promise<PreparedCollabRoom>"
/>

<SourceLink href="/source/plugin/obsync/src/collab/collab-ts/#L192" label="collab.ts:192" />

**Modifiers:** `async`

Doesn't connect yet: call `connect()` once the editor still shows this file. Regular users edit a private doc that only receives network updates, so nothing leaks upstream.

**Parameters**

- `fileName` (string)
- `user` ([CollaborationUser](/module/plugin-obsync-src-collab-collab/types/collaborationuser))
- `requestWebSocketTicket` (() => Promise\<string>)
- `onUserJoined` ((name: string) => void)
- `onUserLeft` ((name: string) => void)

**Returns**

- `Promise<`[`PreparedCollabRoom`](/module/plugin-obsync-src-collab-collab/types/preparedcollabroom)`>`

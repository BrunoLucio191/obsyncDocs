---
title: CollaborationController
kind: class
longname: CollaborationController
description: Keeps a single Yjs room open, for the active Markdown file.
---

# CollaborationController

<SourceLink href="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L14" label="CollaborationController.ts:14" />

Keeps a single Yjs room open, for the active Markdown file.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new CollaborationController(
	app: App,
	auth: CollaborationAuth,
): CollaborationController"
/>

**Parameters**

- `app` (App)
- `auth` ([CollaborationAuth](/collaborationauth))

**Returns**

`CollaborationController`

---

## Properties

<MemberHeading id="editorextensions" depth="3" name="editorExtensions" sig="editorExtensions: Extension[]" />

<MemberMeta badges="readonly" sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L15" sourceLabel="CollaborationController.ts:15" />

**Default:** `[]`

## Accessors

<MemberHeading id="currentpath" depth="3" name="currentPath" sig="get currentPath(): string" />

<MemberMeta sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L28" sourceLabel="CollaborationController.ts:28" />

## Methods

<MemberHeading id="destroy" depth="3" name="destroy" sig="destroy(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L140" sourceLabel="CollaborationController.ts:140" />

**Returns**

- `void`

<MemberHeading id="disconnect" depth="3" name="disconnect" sig="disconnect(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L50" sourceLabel="CollaborationController.ts:50" />

**Returns**

- `void`

<MemberHeading id="disconnectifaffected" depth="3" name="disconnectIfAffected" sig="disconnectIfAffected(path: string): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L65" sourceLabel="CollaborationController.ts:65" />

Also when `path` is a folder above the active file.

**Parameters**

- `path` (string)

**Returns**

- `void`

<MemberHeading id="join" depth="3" name="join" sig="join(filePath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L75" sourceLabel="CollaborationController.ts:75" />

Gives up if the editor switched files or a newer join/disconnect took over while it was loading.

**Parameters**

- `filePath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="refreshafterprofilechange" depth="3" name="refreshAfterProfileChange" sig="refreshAfterProfileChange(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L44" sourceLabel="CollaborationController.ts:44" />

**Returns**

- `void`

<MemberHeading id="scheduleactiveroomsync" depth="3" name="scheduleActiveRoomSync" sig="scheduleActiveRoomSync(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/collab/collaborationcontroller-ts/#L32" sourceLabel="CollaborationController.ts:32" />

**Returns**

- `void`

---
title: YjsPersistence
kind: class
longname: module:backend/yjs/YjsPersistence.YjsPersistence
description: "Saves each document twice: the binary Yjs state (the authority) and a markdown mirror in the vault, so the files stay readable outside the app."
---

# YjsPersistence

<SourceLink href="/source/backend/yjs/yjspersistence-ts/#L29" label="YjsPersistence.ts:29" />

Saves each document twice: the binary Yjs state (the authority) and a markdown mirror in the vault, so the files stay readable outside the app.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new YjsPersistence(
	vaultPath: string,
	statePath: string,
	collaborationServer: YjsCollaborationServer,
): YjsPersistence"
/>

**Parameters**

- `vaultPath` (string)
- `statePath` (string)
- `collaborationServer` ([YjsCollaborationServer](/module/backend-yjs-yjscollaborationserver/yjscollaborationserver))

**Returns**

`YjsPersistence`

---

## Methods

<MemberHeading id="bindstate" depth="3" name="bindState" sig="bindState(docPath: string, ydoc: Doc): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L50" sourceLabel="YjsPersistence.ts:50" />

Decode the file name, reads the binary state , apply the binary update and bind the Y.doc to the state inside a map

**Parameters**

- `docPath` (string) — docName is the path
- `ydoc` (Doc) — the ydoc document that is shared between users

**Returns**

- `Promise<void>`

<MemberHeading id="deletestateunderpath" depth="3" name="deleteStateUnderPath" sig="deleteStateUnderPath(targetPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L109" sourceLabel="YjsPersistence.ts:109" />

Delete a files or whole folder and the directories inside of it

**Parameters**

- `targetPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="destroystate" depth="3" name="destroyState" sig="destroyState(_docName: string, ydoc: Doc): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L97" sourceLabel="YjsPersistence.ts:97" />

**Parameters**

- `_docName` (string)
- `ydoc` (Doc)

**Returns**

- `Promise<void>`

<MemberHeading id="renamestatepath" depth="3" name="renameStatePath" sig="renameStatePath(oldPath: string, newPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L127" sourceLabel="YjsPersistence.ts:127" />

Keeps the collaboration history across a vault rename.

**Parameters**

- `oldPath` (string)
- `newPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="writestate" depth="3" name="writeState" sig="writeState(docPath: string, ydoc: Doc): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L90" sourceLabel="YjsPersistence.ts:90" />

**Parameters**

- `docPath` (string)
- `ydoc` (Doc)

**Returns**

- `Promise<void>`

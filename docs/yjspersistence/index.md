---
title: YjsPersistence
kind: class
longname: YjsPersistence
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
- `collaborationServer` ([YjsCollaborationServer](/yjscollaborationserver))

**Returns**

`YjsPersistence`

---

## Methods

<MemberHeading id="bindstate" depth="3" name="bindState" sig="bindState(docName: string, ydoc: Doc): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L45" sourceLabel="YjsPersistence.ts:45" />

**Parameters**

- `docName` (string)
- `ydoc` (Doc)

**Returns**

- `Promise<void>`

<MemberHeading id="deletestateunderpath" depth="3" name="deleteStateUnderPath" sig="deleteStateUnderPath(targetPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L102" sourceLabel="YjsPersistence.ts:102" />

File or whole folder, so old state can't resurface if the path is reused.

**Parameters**

- `targetPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="destroystate" depth="3" name="destroyState" sig="destroyState(_docName: string, ydoc: Doc): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L92" sourceLabel="YjsPersistence.ts:92" />

**Parameters**

- `_docName` (string)
- `ydoc` (Doc)

**Returns**

- `Promise<void>`

<MemberHeading id="renamestatepath" depth="3" name="renameStatePath" sig="renameStatePath(oldPath: string, newPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L114" sourceLabel="YjsPersistence.ts:114" />

Keeps the collaboration history across a vault rename.

**Parameters**

- `oldPath` (string)
- `newPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="writestate" depth="3" name="writeState" sig="writeState(docName: string, ydoc: Doc): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistence-ts/#L85" sourceLabel="YjsPersistence.ts:85" />

**Parameters**

- `docName` (string)
- `ydoc` (Doc)

**Returns**

- `Promise<void>`

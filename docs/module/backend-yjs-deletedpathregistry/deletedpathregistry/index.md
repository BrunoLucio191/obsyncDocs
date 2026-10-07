---
title: DeletedPathRegistry
kind: class
longname: module:backend/yjs/DeletedPathRegistry.DeletedPathRegistry
description: Lets new connections be refused and rooms be stopped even while a room creation or flush is still running.
---

# DeletedPathRegistry

<SourceLink href="/source/backend/yjs/deletedpathregistry-ts/#L9" label="DeletedPathRegistry.ts:9" />

Lets new connections be refused and rooms be stopped even while a room creation or flush is still running.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new DeletedPathRegistry(): DeletedPathRegistry" />

**Returns**

`DeletedPathRegistry`

---

## Methods

<MemberHeading id="checkifismarked" depth="3" name="checkIfIsMarked" sig="checkIfIsMarked(targetPath: string): boolean" />

<MemberMeta sourceHref="/source/backend/yjs/deletedpathregistry-ts/#L22" sourceLabel="DeletedPathRegistry.ts:22" />

**Parameters**

- `targetPath` (string)

**Returns**

- `boolean`

<MemberHeading id="cleardeleted" depth="3" name="clearDeleted" sig="clearDeleted(targetPath: string): void" />

<MemberMeta sourceHref="/source/backend/yjs/deletedpathregistry-ts/#L46" sourceLabel="DeletedPathRegistry.ts:46" />

Also clears deleted roots above or below it, when a file is recreated.

**Parameters**

- `targetPath` (string)

**Returns**

- `void`

<MemberHeading id="invalidatedocument" depth="3" name="invalidateDocument" sig="invalidateDocument(doc: Doc): void" />

<MemberMeta sourceHref="/source/backend/yjs/deletedpathregistry-ts/#L63" sourceLabel="DeletedPathRegistry.ts:63" />

**Parameters**

- `doc` (Doc)

**Returns**

- `void`

<MemberHeading id="isdocumentinvalidated" depth="3" name="isDocumentInvalidated" sig="isDocumentInvalidated(doc: Doc): boolean" />

<MemberMeta sourceHref="/source/backend/yjs/deletedpathregistry-ts/#L59" sourceLabel="DeletedPathRegistry.ts:59" />

**Parameters**

- `doc` (Doc)

**Returns**

- `boolean`

<MemberHeading id="ispathdeleted" depth="3" name="isPathDeleted" sig="isPathDeleted(filePath: string): boolean" />

<MemberMeta sourceHref="/source/backend/yjs/deletedpathregistry-ts/#L13" sourceLabel="DeletedPathRegistry.ts:13" />

**Parameters**

- `filePath` (string)

**Returns**

- `boolean`

<MemberHeading id="markdeleted" depth="3" name="markDeleted" sig="markDeleted(targetPath: string): string" />

<MemberMeta sourceHref="/source/backend/yjs/deletedpathregistry-ts/#L32" sourceLabel="DeletedPathRegistry.ts:32" />

Already-deleted descendants fold into this new root.

**Parameters**

- `targetPath` (string)

**Returns**

- `string`

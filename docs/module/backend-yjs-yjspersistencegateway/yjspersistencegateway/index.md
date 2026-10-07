---
title: YjsPersistenceGateway
kind: class
longname: module:backend/yjs/YjsPersistenceGateway.YjsPersistenceGateway
description: Every call is a no-op until setAdapter , so callers never check for an adapter.
---

# YjsPersistenceGateway

<SourceLink href="/source/backend/yjs/yjspersistencegateway-ts/#L5" label="YjsPersistenceGateway.ts:5" />

Every call is a no-op until `setAdapter`, so callers never check for an adapter.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new YjsPersistenceGateway(): YjsPersistenceGateway" />

**Returns**

`YjsPersistenceGateway`

---

## Methods

<MemberHeading id="bindstate" depth="3" name="bindState" sig="bindState(docName: string, doc: Doc): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistencegateway-ts/#L12" sourceLabel="YjsPersistenceGateway.ts:12" />

**Parameters**

- `docName` (string)
- `doc` (Doc)

**Returns**

- `Promise<void>`

<MemberHeading id="deletestateunderpath" depth="3" name="deleteStateUnderPath" sig="deleteStateUnderPath(targetPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistencegateway-ts/#L24" sourceLabel="YjsPersistenceGateway.ts:24" />

**Parameters**

- `targetPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="destroystate" depth="3" name="destroyState" sig="destroyState(docName: string, doc: Doc): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistencegateway-ts/#L20" sourceLabel="YjsPersistenceGateway.ts:20" />

**Parameters**

- `docName` (string)
- `doc` (Doc)

**Returns**

- `Promise<void>`

<MemberHeading id="renamestatepath" depth="3" name="renameStatePath" sig="renameStatePath(oldPath: string, newPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistencegateway-ts/#L28" sourceLabel="YjsPersistenceGateway.ts:28" />

**Parameters**

- `oldPath` (string)
- `newPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="setadapter" depth="3" name="setAdapter" sig="setAdapter(adapter: YjsPersistenceAdapter): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjspersistencegateway-ts/#L8" sourceLabel="YjsPersistenceGateway.ts:8" />

**Parameters**

- `adapter` ([YjsPersistenceAdapter](/module/backend-yjs-yjs/types/yjspersistenceadapter))

**Returns**

- `void`

<MemberHeading id="writestate" depth="3" name="writeState" sig="writeState(docName: string, doc: Doc): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/yjs/yjspersistencegateway-ts/#L16" sourceLabel="YjsPersistenceGateway.ts:16" />

**Parameters**

- `docName` (string)
- `doc` (Doc)

**Returns**

- `Promise<void>`

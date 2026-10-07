---
title: SyncBaseStore
kind: class
longname: module:plugin/obSync/src/vault/SyncBaseStore.SyncBaseStore
description: "The last server version of each file a regular user received (the merge base): an index of path -> hash, plus text versions stored by hash."
---

# SyncBaseStore

<SourceLink href="/source/plugin/obsync/src/vault/syncbasestore-ts/#L9" label="SyncBaseStore.ts:9" />

The last server version of each file a regular user received (the merge base): an index of path -> hash, plus text versions stored by hash.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new SyncBaseStore(
	adapter: DataAdapter,
	dir: string,
): SyncBaseStore"
/>

**Parameters**

- `adapter` (DataAdapter)
- `dir` (string)

**Returns**

`SyncBaseStore`

---

## Methods

<MemberHeading id="forget" depth="3" name="forget" sig="forget(path: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/syncbasestore-ts/#L75" sourceLabel="SyncBaseStore.ts:75" />

**Parameters**

- `path` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="gethash" depth="3" name="getHash" sig="getHash(path: string): Promise<string>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/syncbasestore-ts/#L30" sourceLabel="SyncBaseStore.ts:30" />

**Parameters**

- `path` (string)

**Returns**

- `Promise<string>`

<MemberHeading id="gettext" depth="3" name="getText" sig="getText(path: string): Promise<string>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/syncbasestore-ts/#L36" sourceLabel="SyncBaseStore.ts:36" />

**Parameters**

- `path` (string)

**Returns**

- `Promise<string>`

<MemberHeading id="rename" depth="3" name="rename" sig="rename(oldPath: string, newPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/syncbasestore-ts/#L61" sourceLabel="SyncBaseStore.ts:61" />

**Parameters**

- `oldPath` (string)
- `newPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="setbinary" depth="3" name="setBinary" sig="setBinary(path: string, hash: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/syncbasestore-ts/#L57" sourceLabel="SyncBaseStore.ts:57" />

**Parameters**

- `path` (string)
- `hash` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="settext" depth="3" name="setText" sig="setText(path: string, text: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/syncbasestore-ts/#L47" sourceLabel="SyncBaseStore.ts:47" />

**Parameters**

- `path` (string)
- `text` (string)

**Returns**

- `Promise<void>`

## Static Methods

<MemberHeading id="hash" depth="3" name="hash" sig="hash(data: string | ArrayBuffer): Promise<string>" />

<MemberMeta badges="static,async" sourceHref="/source/plugin/obsync/src/vault/syncbasestore-ts/#L19" sourceLabel="SyncBaseStore.ts:19" />

**Parameters**

- `data` (string | ArrayBuffer)

**Returns**

- `Promise<string>`

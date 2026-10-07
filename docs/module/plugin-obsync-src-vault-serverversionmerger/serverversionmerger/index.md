---
title: ServerVersionMerger
kind: class
longname: module:plugin/obSync/src/vault/ServerVersionMerger.ServerVersionMerger
description: Applies a server version of a file to a regular user's vault without losing their private edits.
---

# ServerVersionMerger

<SourceLink href="/source/plugin/obsync/src/vault/serverversionmerger-ts/#L13" label="ServerVersionMerger.ts:13" />

Applies a server version of a file to a regular user's vault without losing their private edits.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new ServerVersionMerger(
	app: App,
	mutedPaths: PathMuteRegistry,
	store: SyncBaseStore,
): ServerVersionMerger"
/>

**Parameters**

- `app` (App)
- `mutedPaths` ([PathMuteRegistry](/module/plugin-obsync-src-vault-pathmuteregistry/pathmuteregistry))
- `store` ([SyncBaseStore](/module/plugin-obsync-src-vault-syncbasestore/syncbasestore))

**Returns**

`ServerVersionMerger`

---

## Methods

<MemberHeading id="apply" depth="3" name="apply" sig="apply(path: string, data: string | ArrayBuffer): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/serverversionmerger-ts/#L28" sourceLabel="ServerVersionMerger.ts:28" />

**Parameters**

- `path` (string)
- `data` (string | ArrayBuffer)

**Returns**

- `Promise<void>`

<MemberHeading id="findmovedcopy" depth="3" name="findMovedCopy" sig="findMovedCopy(oldPath: string): Promise<string>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/serverversionmerger-ts/#L53" sourceLabel="ServerVersionMerger.ts:53" />

Where the user moved `oldPath` without editing it: a file with the same name and content as its base. Files with a base of their own are synced files, not that copy.

**Parameters**

- `oldPath` (string)

**Returns**

- `Promise<string>`

<MemberHeading id="forget" depth="3" name="forget" sig="forget(path: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/serverversionmerger-ts/#L75" sourceLabel="ServerVersionMerger.ts:75" />

**Parameters**

- `path` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="rename" depth="3" name="rename" sig="rename(oldPath: string, newPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/serverversionmerger-ts/#L71" sourceLabel="ServerVersionMerger.ts:71" />

**Parameters**

- `oldPath` (string)
- `newPath` (string)

**Returns**

- `Promise<void>`

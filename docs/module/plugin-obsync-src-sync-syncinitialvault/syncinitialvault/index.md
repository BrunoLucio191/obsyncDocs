---
title: SyncInitialVault
kind: class
longname: module:plugin/obSync/src/sync/SyncInitialVault.SyncInitialVault
description: Downloads the whole vault as a zip and writes it into the local vault.
---

# SyncInitialVault

<SourceLink href="/source/plugin/obsync/src/sync/syncinitialvault-ts/#L10" label="SyncInitialVault.ts:10" />

Downloads the whole vault as a zip and writes it into the local vault.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new SyncInitialVault(
	app: App,
	auth: AuthService,
	mutedPaths: PathMuteRegistry,
	queueManager: QueueManager,
	merger: ServerVersionMerger,
): SyncInitialVault"
/>

**Parameters**

- `app` (App)
- `auth` (AuthService)
- `mutedPaths` ([PathMuteRegistry](/module/plugin-obsync-src-vault-pathmuteregistry/pathmuteregistry))
- `queueManager` (QueueManager)
- `merger` ([ServerVersionMerger](/module/plugin-obsync-src-vault-serverversionmerger/serverversionmerger))

**Returns**

`SyncInitialVault`

---

## Methods

<MemberHeading id="sync" depth="3" name="sync" sig="sync(): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/sync/syncinitialvault-ts/#L32" sourceLabel="SyncInitialVault.ts:32" />

**Returns**

- `Promise<void>`

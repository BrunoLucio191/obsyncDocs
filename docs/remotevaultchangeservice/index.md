---
title: RemoteVaultChangeService
kind: class
longname: RemoteVaultChangeService
description: Applies vault changes from other clients, muting each path so the local event isn't republished. Regular users never publish, so their files go through ServerVersionMerger.
---

# RemoteVaultChangeService

<SourceLink href="/source/plugin/obsync/src/vault/remotevaultchangeservice-ts/#L16" label="RemoteVaultChangeService.ts:16" />

Applies vault changes from other clients, muting each path so the local event isn't republished. Regular users never publish, so their files go through ServerVersionMerger.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new RemoteVaultChangeService(
	app: App,
	auth: AuthService,
	mutedPaths: PathMuteRegistry,
	collaboration: CollaborationController,
	queueManager: QueueManager,
	merger: ServerVersionMerger,
	requestFullSync: () => void,
): RemoteVaultChangeService"
/>

**Parameters**

- `app` (App)
- `auth` ([AuthService](/authservice))
- `mutedPaths` ([PathMuteRegistry](/pathmuteregistry))
- `collaboration` ([CollaborationController](/collaborationcontroller))
- `queueManager` ([QueueManager](/queuemanager))
- `merger` ([ServerVersionMerger](/serverversionmerger))
- `requestFullSync` (() => void)

**Returns**

`RemoteVaultChangeService`

---

## Methods

<MemberHeading id="apply" depth="3" name="apply" sig="apply(change: VaultChange): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/vault/remotevaultchangeservice-ts/#L47" sourceLabel="RemoteVaultChangeService.ts:47" />

Add changes inside the client queue

**Parameters**

- `change` ([VaultChange](/vaultchange))

**Returns**

- `Promise<void>`

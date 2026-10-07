---
title: SystemChannel
kind: class
longname: module:plugin/obSync/src/sync/SystemChannel.SystemChannel
description: Websocket to /system , where the backend broadcasts vault changes made by other clients.
---

# SystemChannel

<SourceLink href="/source/plugin/obsync/src/sync/systemchannel-ts/#L18" label="SystemChannel.ts:18" />

Websocket to `/system`, where the backend broadcasts vault changes made by other clients.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new SystemChannel(
	auth: AuthService,
	remoteChanges: RemoteVaultChangeService,
	app: App,
	initialVaultSync: SyncInitialVault,
): SystemChannel"
/>

**Parameters**

- `auth` (AuthService)
- `remoteChanges` ([RemoteVaultChangeService](/module/plugin-obsync-src-vault-remotevaultchangeservice/remotevaultchangeservice))
- `app` (App)
- `initialVaultSync` ([SyncInitialVault](/module/plugin-obsync-src-sync-syncinitialvault/syncinitialvault))

**Returns**

`SystemChannel`

---

## Methods

<MemberHeading id="connect" depth="3" name="connect" sig="connect(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/sync/systemchannel-ts/#L41" sourceLabel="SystemChannel.ts:41" />

**Returns**

- `void`

<MemberHeading id="disconnect" depth="3" name="disconnect" sig="disconnect(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/sync/systemchannel-ts/#L47" sourceLabel="SystemChannel.ts:47" />

**Returns**

- `void`

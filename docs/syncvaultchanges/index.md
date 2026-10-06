---
title: SyncVaultChanges
kind: class
longname: SyncVaultChanges
description: Publishes an admin's local vault events, one queue task each. Paths are read when the event fires, because Obsidian renames the same file object in place.
---

# SyncVaultChanges

<SourceLink href="/source/plugin/obsync/src/sync/syncvaultchanges-ts/#L20" label="SyncVaultChanges.ts:20" />

Publishes an admin's local vault events, one queue task each. Paths are read when the event fires, because Obsidian renames the same file object in place.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new SyncVaultChanges(
	plugin: Plugin,
	auth: AuthService,
	mutedPaths: PathMuteRegistry,
	collaboration: CollaborationController,
	queueManager: QueueManager,
): SyncVaultChanges"
/>

**Parameters**

- `plugin` (Plugin)
- `auth` ([AuthService](/authservice))
- `mutedPaths` ([PathMuteRegistry](/pathmuteregistry))
- `collaboration` ([CollaborationController](/collaborationcontroller))
- `queueManager` ([QueueManager](/queuemanager))

**Returns**

`SyncVaultChanges`

---

## Methods

<MemberHeading id="initialize" depth="3" name="initialize" sig="initialize(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/sync/syncvaultchanges-ts/#L43" sourceLabel="SyncVaultChanges.ts:43" />

**Returns**

- `void`

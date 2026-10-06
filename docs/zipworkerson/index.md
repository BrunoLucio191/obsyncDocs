---
title: ZipWorkerSon
kind: class
longname: ZipWorkerSon
description: Downloads on the main thread (the only one with the Obsidian API) and unzips in a Worker. Skipped while the gene saved after the last complete sync still matches the server's.
---

# ZipWorkerSon

<SourceLink href="/source/plugin/obsync/src/workers/zipworker/zipworkerson-ts/#L18" label="ZipWorkerSon.ts:18" />

Downloads on the main thread (the only one with the Obsidian API) and unzips in a Worker. Skipped while the gene saved after the last complete sync still matches the server's.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new ZipWorkerSon(
	app: App,
	mutedPath: PathMuteRegistry,
	auth: AuthService,
	queueManager: QueueManager,
	merger: ServerVersionMerger,
): ZipWorkerSon"
/>

**Parameters**

- `app` (App)
- `mutedPath` ([PathMuteRegistry](/pathmuteregistry))
- `auth` ([AuthService](/authservice))
- `queueManager` ([QueueManager](/queuemanager))
- `merger` ([ServerVersionMerger](/serverversionmerger))

**Returns**

`ZipWorkerSon`

---

## Methods

<MemberHeading id="startworking" depth="3" name="startWorking" sig="startWorking(): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/workers/zipworker/zipworkerson-ts/#L40" sourceLabel="ZipWorkerSon.ts:40" />

**Returns**

- `Promise<void>`

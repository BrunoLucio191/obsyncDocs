---
title: PathMuteRegistry
kind: class
longname: PathMuteRegistry
description: Paths the plugin itself is about to change, so the resulting vault event isn't published back to the server. Mutes expire on their own.
---

# PathMuteRegistry

<SourceLink href="/source/plugin/obsync/src/vault/pathmuteregistry-ts/#L5" label="PathMuteRegistry.ts:5" />

Paths the plugin itself is about to change, so the resulting vault event isn't published back to the server. Mutes expire on their own.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new PathMuteRegistry(muteDurationMs: number): PathMuteRegistry" />

**Parameters**

- `muteDurationMs` (number, default: "2_000")

**Returns**

`PathMuteRegistry`

---

## Methods

<MemberHeading id="clear" depth="3" name="clear" sig="clear(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/vault/pathmuteregistry-ts/#L30" sourceLabel="PathMuteRegistry.ts:30" />

**Returns**

- `void`

<MemberHeading id="ismuted" depth="3" name="isMuted" sig="isMuted(path: string): boolean" />

<MemberMeta sourceHref="/source/plugin/obsync/src/vault/pathmuteregistry-ts/#L20" sourceLabel="PathMuteRegistry.ts:20" />

A muted folder mutes everything under it.

**Parameters**

- `path` (string)

**Returns**

- `boolean`

<MemberHeading id="mute" depth="3" name="mute" sig="mute(path: string): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/vault/pathmuteregistry-ts/#L15" sourceLabel="PathMuteRegistry.ts:15" />

Mute a path so the changes made on him are not published back

**Parameters**

- `path` (string)

**Returns**

- `void`

## Static Methods

<MemberHeading id="contains" depth="3" name="contains" sig="contains(rootPath: string, candidatePath: string): boolean" />

<MemberMeta badges="static" sourceHref="/source/plugin/obsync/src/vault/pathmuteregistry-ts/#L34" sourceLabel="PathMuteRegistry.ts:34" />

**Parameters**

- `rootPath` (string)
- `candidatePath` (string)

**Returns**

- `boolean`

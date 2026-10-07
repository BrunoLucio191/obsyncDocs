---
title: ensureParentFolder
kind: function
longname: module:plugin/obSync/src/vault/ensureParentFolder.ensureParentFolder
description: Creates the missing parent folders of a file, muting each so its event isn't republished.
---

# ensureParentFolder

<Signature
  code="ensureParentFolder(
	adapter: DataAdapter,
	mutedPaths: PathMuteRegistry,
	filePath: string,
): Promise<void>"
/>

<SourceLink href="/source/plugin/obsync/src/vault/ensureparentfolder-ts/#L5" label="ensureParentFolder.ts:5" />

**Modifiers:** `async`

Creates the missing parent folders of a file, muting each so its event isn't republished.

**Parameters**

- `adapter` (DataAdapter)
- `mutedPaths` ([PathMuteRegistry](/module/plugin-obsync-src-vault-pathmuteregistry/pathmuteregistry))
- `filePath` (string)

**Returns**

- `Promise<void>`

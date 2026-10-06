---
title: FileManager
kind: class
longname: FileManager
description: Every path is validated first, so absolute paths or .. can't escape the vault.
---

# FileManager

<SourceLink href="/source/backend/server/filemanager-ts/#L9" label="FileManager.ts:9" />

Every path is validated first, so absolute paths or `..` can't escape the vault.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new FileManager(): FileManager" />

**Returns**

`FileManager`

---

## Methods

<MemberHeading id="createfolder" depth="3" name="createFolder" sig="createFolder(folderPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/filemanager-ts/#L70" sourceLabel="FileManager.ts:70" />

**Parameters**

- `folderPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading
  id="createormodifyfile"
  depth="3"
  name="createOrModifyFile"
  sig="createOrModifyFile(
	filePath: string,
	content: string | Buffer<ArrayBuffer>,
): Promise<void>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/server/filemanager-ts/#L39" sourceLabel="FileManager.ts:39" />

**Parameters**

- `filePath` (string)
- `content` (string | Buffer\<ArrayBuffer>)

**Returns**

- `Promise<void>`

<MemberHeading id="deletepath" depth="3" name="deletePath" sig="deletePath(targetPath: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/filemanager-ts/#L75" sourceLabel="FileManager.ts:75" />

**Parameters**

- `targetPath` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="directoryziped" depth="3" name="directoryZiped" sig="directoryZiped(zipPath: string, clientId: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/filemanager-ts/#L99" sourceLabel="FileManager.ts:99" />

**Parameters**

- `zipPath` (string)
- `clientId` (string)

**Returns**

- `Promise<void>`

<MemberHeading id="getfilepath" depth="3" name="getFilePath" sig="getFilePath(filePath: string): Promise<string>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/filemanager-ts/#L51" sourceLabel="FileManager.ts:51" />

`null` for folders, missing paths and paths outside the vault.

**Parameters**

- `filePath` (string)

**Returns**

- `Promise<string>`

<MemberHeading id="isfolder" depth="3" name="isFolder" sig="isFolder(folderPath: string): Promise<boolean>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/filemanager-ts/#L60" sourceLabel="FileManager.ts:60" />

**Parameters**

- `folderPath` (string)

**Returns**

- `Promise<boolean>`

<MemberHeading
  id="rename"
  depth="3"
  name="rename"
  sig="rename(
	oldPath: string,
	newPath: string,
): Promise<'moved' | 'already-applied' | 'not-found'>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/server/filemanager-ts/#L84" sourceLabel="FileManager.ts:84" />

Already applied when only the destination exists: Obsidian reports each descendant of a moved folder after the folder itself. Not found means the source never reached the vault.

**Parameters**

- `oldPath` (string)
- `newPath` (string)

**Returns**

- `Promise<"moved" | "already-applied" | "not-found">`

<MemberHeading id="stringtofile" depth="3" name="stringToFile" sig="stringToFile(fileContent: string, name: string): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/filemanager-ts/#L35" sourceLabel="FileManager.ts:35" />

**Parameters**

- `fileContent` (string)
- `name` (string)

**Returns**

- `Promise<void>`

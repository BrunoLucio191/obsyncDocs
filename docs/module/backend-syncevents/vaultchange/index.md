---
title: VaultChange
kind: typedef
longname: module:backend/syncEvents.VaultChange
description: originClientId lets the client that made the change ignore its own echo.
---

# VaultChange

<Signature code="VaultChange = { content?: string; isBinary?: boolean; isFolder: boolean; originClientId?: string; path: string; type: 'create' } | { isFolder: boolean; originClientId?: string; path: string; type: 'delete' } | { content: string; originClientId?: string; path: string; type: 'modify' } | { isFolder: boolean; newPath: string; oldPath: string; originClientId?: string; type: 'rename' }" />

<SourceLink href="/source/backend/syncevents-ts/#L4" label="syncEvents.ts:4" />

`originClientId` lets the client that made the change ignore its own echo.

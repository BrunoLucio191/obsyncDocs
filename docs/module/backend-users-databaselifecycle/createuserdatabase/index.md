---
title: createUserDatabase
kind: function
longname: module:backend/users/databaseLifecycle.createUserDatabase
description: A failed setup removes the partial file and its WAL/SHM sidecars, so no corrupt database is left.
---

# createUserDatabase

<Signature code="createUserDatabase(databasePath: string): Promise<void>" />

<SourceLink href="/source/backend/users/databaselifecycle-ts/#L39" label="databaseLifecycle.ts:39" />

**Modifiers:** `async`

A failed setup removes the partial file and its WAL/SHM sidecars, so no corrupt database is left.

**Parameters**

- `databasePath` (string)

**Returns**

- `Promise<void>`

---
title: KeyedLock
kind: class
longname: module:backend/queue/KeyedLock.KeyedLock
description: Two tasks with the same key never run at once, even in different queues. A key names an operation on a resource, e.g. user:42:renameUser .
---

# KeyedLock

<SourceLink href="/source/backend/queue/keyedlock-ts/#L5" label="KeyedLock.ts:5" />

Two tasks with the same key never run at once, even in different queues. A key names an operation on a resource, e.g. `user:42:renameUser`.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new KeyedLock(): KeyedLock" />

**Returns**

`KeyedLock`

---

## Accessors

<MemberHeading id="busykeys" depth="3" name="busyKeys" sig="get busyKeys(): number" />

<MemberMeta sourceHref="/source/backend/queue/keyedlock-ts/#L37" sourceLabel="KeyedLock.ts:37" />

## Methods

<MemberHeading id="run" depth="3" name="run" sig="run<T>(operation: () => Promise<T>, key: string): Promise<T>" />

<MemberMeta badges="async" sourceHref="/source/backend/queue/keyedlock-ts/#L8" sourceLabel="KeyedLock.ts:8" />

**Type Parameters**

- `T`

**Parameters**

- `operation` (() => Promise\<T>)
- `key` (string)

**Returns**

- `Promise<T>`

---
title: Queue
kind: class
longname: Queue
description: Runs tasks one at a time, in arrival order. Each task first takes the shared KeyedLock for its key, so it waits while another queue runs something with the same key.
---

# Queue

<SourceLink href="/source/backend/queue/queue-ts/#L7" label="Queue.ts:7" />

Runs tasks one at a time, in arrival order. Each task first takes the shared KeyedLock for its key, so it waits while another queue runs something with the same key.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new Queue(lock: KeyedLock, onEmpty?: () => void): Queue" />

**Parameters**

- `lock` ([KeyedLock](/keyedlock))
- `onEmpty` (() => void, optional)

**Returns**

`Queue`

---

## Accessors

<MemberHeading id="gettaskidentifiers" depth="3" name="getTaskIdentifiers" sig="get getTaskIdentifiers(): string[]" />

<MemberMeta sourceHref="/source/backend/queue/queue-ts/#L74" sourceLabel="Queue.ts:74" />

<MemberHeading id="isprocessing" depth="3" name="isProcessing" sig="get isProcessing(): boolean" />

<MemberMeta sourceHref="/source/backend/queue/queue-ts/#L78" sourceLabel="Queue.ts:78" />

<MemberHeading id="numberoftaks" depth="3" name="numberOfTaks" sig="get numberOfTaks(): number" />

<MemberMeta sourceHref="/source/backend/queue/queue-ts/#L70" sourceLabel="Queue.ts:70" />

<MemberHeading id="gettaskidentifiers" depth="3" name="getTaskIdentifiers" sig="get getTaskIdentifiers(): string[]" />

<MemberMeta sourceHref="/source/plugin/obsync/src/queue/queue-ts/#L73" sourceLabel="Queue.ts:73" />

<MemberHeading id="isprocessing" depth="3" name="isProcessing" sig="get isProcessing(): boolean" />

<MemberMeta sourceHref="/source/plugin/obsync/src/queue/queue-ts/#L77" sourceLabel="Queue.ts:77" />

<MemberHeading id="numberoftaks" depth="3" name="numberOfTaks" sig="get numberOfTaks(): number" />

<MemberMeta sourceHref="/source/plugin/obsync/src/queue/queue-ts/#L69" sourceLabel="Queue.ts:69" />

## Methods

<MemberHeading id="addtask" depth="3" name="addTask" sig="addTask<T>(task: () => Promise<T>, taskKey: string): Promise<T>" />

<MemberMeta badges="async" sourceHref="/source/backend/queue/queue-ts/#L18" sourceLabel="Queue.ts:18" />

**Type Parameters**

- `T`

**Parameters**

- `task` (() => Promise\<T>)
- `taskKey` (string)

**Returns**

- `Promise<T>`

<MemberHeading id="addtask" depth="3" name="addTask" sig="addTask<T>(task: () => Promise<T>, taskKey: string): Promise<T>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/queue/queue-ts/#L18" sourceLabel="Queue.ts:18" />

**Type Parameters**

- `T`

**Parameters**

- `task` (() => Promise\<T>)
- `taskKey` (string)

**Returns**

- `Promise<T>`

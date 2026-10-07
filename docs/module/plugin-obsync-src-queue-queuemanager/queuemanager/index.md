---
title: QueueManager
kind: class
longname: module:plugin/obSync/src/queue/QueueManager.QueueManager
description: One queue per user, all sharing the same KeyedLock. A queue is removed once it drains, so add the task right after getOrCreateQueue instead of holding the queue across an await.
---

# QueueManager

<SourceLink href="/source/plugin/obsync/src/queue/queuemanager-ts/#L8" label="QueueManager.ts:8" />

One queue per user, all sharing the same KeyedLock. A queue is removed once it drains, so add the task right after getOrCreateQueue instead of holding the queue across an await.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new QueueManager(lock: KeyedLock): QueueManager" />

**Parameters**

- `lock` (KeyedLock)

**Returns**

`QueueManager`

---

## Methods

<MemberHeading id="getorcreatequeue" depth="3" name="getOrCreateQueue" sig="getOrCreateQueue(userId: string): default" />

<MemberMeta sourceHref="/source/plugin/obsync/src/queue/queuemanager-ts/#L16" sourceLabel="QueueManager.ts:16" />

**Parameters**

- `userId` (string)

**Returns**

- `default`

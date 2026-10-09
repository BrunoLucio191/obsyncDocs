---
title: UserDirectory
kind: class
longname: module:plugin/obSync/src/settings/users/UserDirectory.UserDirectory
description: Local copy of the user list, updated after each action so the UI doesn't re-fetch it.
---

# UserDirectory

<SourceLink href="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L4" label="UserDirectory.ts:4" />

Local copy of the user list, updated after each action so the UI doesn't re-fetch it.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new UserDirectory(): UserDirectory" />

**Returns**

`UserDirectory`

---

## Accessors

<MemberHeading id="size" depth="3" name="size" sig="get size(): number" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L79" sourceLabel="UserDirectory.ts:79" />

## Methods

<MemberHeading id="activeadmincount" depth="3" name="activeAdminCount" sig="activeAdminCount(): number" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L69" sourceLabel="UserDirectory.ts:69" />

Count the number of admins in the plugin

**Returns**

- `number`

<MemberHeading id="add" depth="3" name="add" sig="add(newUser: AuthenticatedUser): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L19" sourceLabel="UserDirectory.ts:19" />

Ignores an id already cached, so a stale double call can't duplicate a row.

**Parameters**

- `newUser` (AuthenticatedUser)

**Returns**

- `void`

<MemberHeading id="all" depth="3" name="all" sig="all(): AuthenticatedUser[]" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L75" sourceLabel="UserDirectory.ts:75" />

Return an array with all users

**Returns**

- `AuthenticatedUser[]`

<MemberHeading id="findbyemail" depth="3" name="findByEmail" sig="findByEmail(email: string): AuthenticatedUser" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L59" sourceLabel="UserDirectory.ts:59" />

**Parameters**

- `email` (string)

**Returns**

- `AuthenticatedUser`

<MemberHeading
  id="findbyname"
  depth="3"
  name="findByName"
  sig="findByName(
	name: string,
	exceptUserId?: number,
): AuthenticatedUser"
/>

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L45" sourceLabel="UserDirectory.ts:45" />

**Parameters**

- `name` (string)
- `exceptUserId` (number, optional)

**Returns**

- `AuthenticatedUser`

<MemberHeading id="remove" depth="3" name="remove" sig="remove(userId: number): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L30" sourceLabel="UserDirectory.ts:30" />

**Parameters**

- `userId` (number)

**Returns**

- `void`

<MemberHeading id="replace" depth="3" name="replace" sig="replace(updatedUser: AuthenticatedUser): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L11" sourceLabel="UserDirectory.ts:11" />

**Parameters**

- `updatedUser` (AuthenticatedUser)

**Returns**

- `void`

<MemberHeading id="replaceall" depth="3" name="replaceAll" sig="replaceAll(users: AuthenticatedUser[]): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L7" sourceLabel="UserDirectory.ts:7" />

**Parameters**

- `users` (AuthenticatedUser\[])

**Returns**

- `void`

<MemberHeading id="search" depth="3" name="search" sig="search(query: string): AuthenticatedUser[]" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userdirectory-ts/#L34" sourceLabel="UserDirectory.ts:34" />

**Parameters**

- `query` (string)

**Returns**

- `AuthenticatedUser[]`

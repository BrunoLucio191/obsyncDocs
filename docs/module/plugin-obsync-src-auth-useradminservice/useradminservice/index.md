---
title: UserAdminService
kind: class
longname: module:plugin/obSync/src/auth/UserAdminService.UserAdminService
description: Client for the admin-only user endpoints.
---

# UserAdminService

<SourceLink href="/source/plugin/obsync/src/auth/useradminservice-ts/#L20" label="UserAdminService.ts:20" />

Client for the admin-only user endpoints.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new UserAdminService(auth: AuthService): UserAdminService" />

**Parameters**

- `auth` (AuthService)

**Returns**

`UserAdminService`

---

## Methods

<MemberHeading
  id="changeuserpassword"
  depth="3"
  name="changeUserPassword"
  sig="changeUserPassword(
	userId: number,
	newPassword: string,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L165" sourceLabel="UserAdminService.ts:165" />

changes user password

**Parameters**

- `userId` (number)
- `newPassword` (string)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading
  id="createuser"
  depth="3"
  name="createUser"
  sig="createUser(
	input: { email: string; name: string; password: string; role: UserRole },
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L71" sourceLabel="UserAdminService.ts:71" />

creates a user

**Parameters**

- `input` ({ email: string; name: string; password: string; role: UserRole })

**Properties**

- `email` (string)
- `name` (string)
- `password` (string)
- `role` (UserRole)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading
  id="deleteuser"
  depth="3"
  name="deleteUser"
  sig="deleteUser(
	userId: number,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L141" sourceLabel="UserAdminService.ts:141" />

deletes an user

**Parameters**

- `userId` (number)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading id="listusers" depth="3" name="listUsers" sig="listUsers(): Promise<UserActionResult<AuthenticatedUser[]>>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L28" sourceLabel="UserAdminService.ts:28" />

list all users

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser[]>>`

<MemberHeading
  id="updateusername"
  depth="3"
  name="updateUserName"
  sig="updateUserName(
	userId: number,
	name: string,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L152" sourceLabel="UserAdminService.ts:152" />

updates the name of an user

**Parameters**

- `userId` (number)
- `name` (string)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading
  id="updateuserrole"
  depth="3"
  name="updateUserRole"
  sig="updateUserRole(
	userId: number,
	role: UserRole,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L117" sourceLabel="UserAdminService.ts:117" />

Updates the user role

**Parameters**

- `userId` (number)
- `role` (UserRole)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading
  id="updateuserstatus"
  depth="3"
  name="updateUserStatus"
  sig="updateUserStatus(
	userId: number,
	active: boolean,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L129" sourceLabel="UserAdminService.ts:129" />

updates an user role

**Parameters**

- `userId` (number)
- `active` (boolean)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

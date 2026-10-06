---
title: UserAdminService
kind: class
longname: UserAdminService
description: Client for the admin-only user endpoints.
---

# UserAdminService

<SourceLink href="/source/plugin/obsync/src/auth/useradminservice-ts/#L18" label="UserAdminService.ts:18" />

Client for the admin-only user endpoints.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new UserAdminService(auth: AuthService): UserAdminService" />

**Parameters**

- `auth` ([AuthService](/authservice))

**Returns**

`UserAdminService`

---

## Methods

<MemberHeading
  id="createuser"
  depth="3"
  name="createUser"
  sig="createUser(
	input: { email: string; name: string; password: string; role: UserRole },
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L62" sourceLabel="UserAdminService.ts:62" />

**Parameters**

- `input` ({ email: string; name: string; password: string; role: [UserRole](/userrole) })

**Properties**

- `email` (string)
- `name` (string)
- `password` (string)
- `role` ([UserRole](/userrole))

**Returns**

- `Promise<`[`UserActionResult`](/useractionresult)`<`[`AuthenticatedUser`](/authenticateduser)`>>`

<MemberHeading
  id="deleteuser"
  depth="3"
  name="deleteUser"
  sig="deleteUser(
	userId: number,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L126" sourceLabel="UserAdminService.ts:126" />

**Parameters**

- `userId` (number)

**Returns**

- `Promise<`[`UserActionResult`](/useractionresult)`<`[`AuthenticatedUser`](/authenticateduser)`>>`

<MemberHeading id="listusers" depth="3" name="listUsers" sig="listUsers(): Promise<UserActionResult<AuthenticatedUser[]>>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L25" sourceLabel="UserAdminService.ts:25" />

**Returns**

- `Promise<`[`UserActionResult`](/useractionresult)`<`[`AuthenticatedUser`](/authenticateduser)`[]>>`

<MemberHeading
  id="resetuserpassword"
  depth="3"
  name="resetUserPassword"
  sig="resetUserPassword(
	userId: number,
	newPassword: string,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L149" sourceLabel="UserAdminService.ts:149" />

**Parameters**

- `userId` (number)
- `newPassword` (string)

**Returns**

- `Promise<`[`UserActionResult`](/useractionresult)`<`[`AuthenticatedUser`](/authenticateduser)`>>`

<MemberHeading
  id="updateusername"
  depth="3"
  name="updateUserName"
  sig="updateUserName(
	userId: number,
	name: string,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L137" sourceLabel="UserAdminService.ts:137" />

**Parameters**

- `userId` (number)
- `name` (string)

**Returns**

- `Promise<`[`UserActionResult`](/useractionresult)`<`[`AuthenticatedUser`](/authenticateduser)`>>`

<MemberHeading
  id="updateuserrole"
  depth="3"
  name="updateUserRole"
  sig="updateUserRole(
	userId: number,
	role: UserRole,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L102" sourceLabel="UserAdminService.ts:102" />

**Parameters**

- `userId` (number)
- `role` ([UserRole](/userrole))

**Returns**

- `Promise<`[`UserActionResult`](/useractionresult)`<`[`AuthenticatedUser`](/authenticateduser)`>>`

<MemberHeading
  id="updateuserstatus"
  depth="3"
  name="updateUserStatus"
  sig="updateUserStatus(
	userId: number,
	active: boolean,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/useradminservice-ts/#L114" sourceLabel="UserAdminService.ts:114" />

**Parameters**

- `userId` (number)
- `active` (boolean)

**Returns**

- `Promise<`[`UserActionResult`](/useractionresult)`<`[`AuthenticatedUser`](/authenticateduser)`>>`

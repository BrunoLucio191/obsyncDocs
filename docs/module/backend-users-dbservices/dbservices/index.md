---
title: DBServices
kind: class
longname: module:backend/users/DBServices.DBServices
description: User CRUD and its rules, e.g. the last active admin can't be demoted, deactivated or deleted.
---

# DBServices

<SourceLink href="/source/backend/users/dbservices-ts/#L19" label="DBServices.ts:19" />

User CRUD and its rules, e.g. the last active admin can't be demoted, deactivated or deleted.

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new DBServices(userDB: UserDB): DBServices" />

**Parameters**

- `userDB` ([UserDB](/module/backend-users-userdb/userdb))

**Returns**

`DBServices`

---

## Methods

<MemberHeading
  id="adminsetuserpassword"
  depth="3"
  name="adminSetUserPassword"
  sig="adminSetUserPassword(
	userId: number,
	newPassword: string,
): Promise<UserMutationResult>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L289" sourceLabel="DBServices.ts:289" />

**Parameters**

- `userId` (number)
- `newPassword` (string)

**Returns**

- `Promise<`[`UserMutationResult`](/module/backend-auth-auth/types/usermutationresult)`>`

<MemberHeading
  id="createuser"
  depth="3"
  name="createUser"
  sig="createUser(
	name: string,
	email: string,
	password: string,
	role: UserRole,
): Promise<CreateUserResult>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L100" sourceLabel="DBServices.ts:100" />

The uniqueness checks and the insert share a transaction, so two requests can't both pass.

**Parameters**

- `name` (string)
- `email` (string)
- `password` (string)
- `role` (UserRole, default: "\\"user\\"")

**Returns**

- `Promise<`[`CreateUserResult`](/module/backend-auth-auth/types/createuserresult)`>`

<MemberHeading id="deleteuser" depth="3" name="deleteUser" sig="deleteUser(userId: number): Promise<UserMutationResult>" />

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L307" sourceLabel="DBServices.ts:307" />

**Parameters**

- `userId` (number)

**Returns**

- `Promise<`[`UserMutationResult`](/module/backend-auth-auth/types/usermutationresult)`>`

<MemberHeading
  id="getuserbyid"
  depth="3"
  name="getUserById"
  sig="getUserById(
	userId: number,
	includeInactive: boolean,
): Promise<AuthenticatedUser>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L79" sourceLabel="DBServices.ts:79" />

**Parameters**

- `userId` (number)
- `includeInactive` (boolean, default: "false")

**Returns**

- `Promise<AuthenticatedUser>`

<MemberHeading id="isuserrole" depth="3" name="isUserRole" sig="isUserRole(value: unknown): value is UserRole" />

<MemberMeta sourceHref="/source/backend/users/dbservices-ts/#L28" sourceLabel="DBServices.ts:28" />

**Parameters**

- `value` (unknown)

**Returns**

- `value is UserRole`

<MemberHeading id="listusers" depth="3" name="listUsers" sig="listUsers(): Promise<AuthenticatedUser[]>" />

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L88" sourceLabel="DBServices.ts:88" />

**Returns**

- `Promise<AuthenticatedUser[]>`

<MemberHeading
  id="rowtouser"
  depth="3"
  name="rowToUser"
  sig="rowToUser(
	row: Omit<StoredUserRow, 'password_hash'>,
): AuthenticatedUser"
/>

<MemberMeta sourceHref="/source/backend/users/dbservices-ts/#L62" sourceLabel="DBServices.ts:62" />

**Parameters**

- `row` (Omit\<[StoredUserRow](/module/backend-auth-auth/types/storeduserrow), "[password_hash](/module/backend-auth-auth/types/storeduserrow#passwordhash)">)

**Returns**

- `AuthenticatedUser`

<MemberHeading id="runimmediatetransaction" depth="3" name="runImmediateTransaction" sig="runImmediateTransaction<T>(operation: () => T): T" />

<MemberMeta sourceHref="/source/backend/users/dbservices-ts/#L50" sourceLabel="DBServices.ts:50" />

**Type Parameters**

- `T`

**Parameters**

- `operation` (() => T)

**Returns**

- `T`

<MemberHeading
  id="updateusercolor"
  depth="3"
  name="updateUserColor"
  sig="updateUserColor(
	userId: number,
	color: string,
): Promise<UserMutationResult>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L180" sourceLabel="DBServices.ts:180" />

Not part of authorization, so no event is emitted and live connections are kept.

**Parameters**

- `userId` (number)
- `color` (string)

**Returns**

- `Promise<`[`UserMutationResult`](/module/backend-auth-auth/types/usermutationresult)`>`

<MemberHeading
  id="updateusername"
  depth="3"
  name="updateUserName"
  sig="updateUserName(
	userId: number,
	name: string,
): Promise<UserMutationResult>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L151" sourceLabel="DBServices.ts:151" />

The name is part of the session's user data, hence the authorization-changed event.

**Parameters**

- `userId` (number)
- `name` (string)

**Returns**

- `Promise<`[`UserMutationResult`](/module/backend-auth-auth/types/usermutationresult)`>`

<MemberHeading
  id="updateuserpassword"
  depth="3"
  name="updateUserPassword"
  sig="updateUserPassword(
	userId: number,
	currentPassword: string,
	newPassword: string,
): Promise<UserMutationResult>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L259" sourceLabel="DBServices.ts:259" />

**Parameters**

- `userId` (number)
- `currentPassword` (string)
- `newPassword` (string)

**Returns**

- `Promise<`[`UserMutationResult`](/module/backend-auth-auth/types/usermutationresult)`>`

<MemberHeading
  id="updateuserrole"
  depth="3"
  name="updateUserRole"
  sig="updateUserRole(
	userId: number,
	role: UserRole,
): Promise<UserMutationResult>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L198" sourceLabel="DBServices.ts:198" />

**Parameters**

- `userId` (number)
- `role` (UserRole)

**Returns**

- `Promise<`[`UserMutationResult`](/module/backend-auth-auth/types/usermutationresult)`>`

<MemberHeading
  id="updateuserstatus"
  depth="3"
  name="updateUserStatus"
  sig="updateUserStatus(
	userId: number,
	active: boolean,
): Promise<UserMutationResult>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/users/dbservices-ts/#L231" sourceLabel="DBServices.ts:231" />

**Parameters**

- `userId` (number)
- `active` (boolean)

**Returns**

- `Promise<`[`UserMutationResult`](/module/backend-auth-auth/types/usermutationresult)`>`

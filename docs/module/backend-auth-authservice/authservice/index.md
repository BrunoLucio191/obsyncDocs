---
title: AuthService
kind: class
longname: module:backend/auth/authService.AuthService
---

# AuthService

<SourceLink href="/source/backend/auth/authservice-ts/#L8" label="authService.ts:8" />

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new AuthService(
	userDB: UserDB,
	dbService: DBServices,
	tokenService: TokenService,
): AuthService"
/>

**Parameters**

- `userDB` ([UserDB](/module/backend-users-userdb/userdb))
- `dbService` ([DBServices](/module/backend-users-dbservices/dbservices))
- `tokenService` ([TokenService](/module/backend-auth-tokenservice/tokenservice))

**Returns**

`AuthService`

---

## Methods

<MemberHeading id="login" depth="3" name="login" sig="login(email: string, password: string): Promise<AuthSession>" />

<MemberMeta badges="async" sourceHref="/source/backend/auth/authservice-ts/#L19" sourceLabel="authService.ts:19" />

**Parameters**

- `email` (string)
- `password` (string)

**Returns**

- `Promise<AuthSession>`

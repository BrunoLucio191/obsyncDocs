---
title: AuthSession
kind: typedef
longname: AuthSession
---

# AuthSession

<Signature
  code="AuthSession = {
	expiresIn: number;
	refreshToken: string;
	token: string;
	user: AuthenticatedUser;
}"
/>

<SourceLink href="/source/backend/auth/auth-types-ts/#L14" label="auth.types.ts:14" />

**Properties**

- `expiresIn` (number) — In seconds.
- `refreshToken` (string)
- `token` (string)
- `user` ([AuthenticatedUser](/authenticateduser))

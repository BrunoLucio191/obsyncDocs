---
title: AuthenticatedUser
kind: typedef
longname: AuthenticatedUser
---

# AuthenticatedUser

<Signature
  code="AuthenticatedUser = {
	active: boolean;
	color: string;
	email: string;
	id: number;
	name: string;
	role: UserRole;
}"
/>

<SourceLink href="/source/backend/auth/auth-types-ts/#L4" label="auth.types.ts:4" />

**Properties**

- `active` (boolean)
- `color` (string) — Lowercase `#rrggbb`.
- `email` (string)
- `id` (number)
- `name` (string)
- `role` ([UserRole](/userrole))

---
title: LoginRateLimiter
kind: class
longname: module:backend/auth/LoginRateLimiter.LoginRateLimiter
description: Sliding window per key (account or IP), kept only in memory.
---

# LoginRateLimiter

<SourceLink href="/source/backend/auth/loginratelimiter-ts/#L26" label="LoginRateLimiter.ts:26" />

Sliding window per key (account or IP), kept only in memory.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new LoginRateLimiter(
	options: LoginRateLimiterOptions,
): LoginRateLimiter"
/>

**Parameters**

- `options` (LoginRateLimiterOptions, default: "{}")

**Returns**

`LoginRateLimiter`

---

## Methods

<MemberHeading id="check" depth="3" name="check" sig="check(key: string): LoginRateLimit" />

<MemberMeta sourceHref="/source/backend/auth/loginratelimiter-ts/#L40" sourceLabel="LoginRateLimiter.ts:40" />

**Parameters**

- `key` (string)

**Returns**

- [`LoginRateLimit`](/module/backend-auth-loginratelimiter/loginratelimit)

<MemberHeading id="recordfailure" depth="3" name="recordFailure" sig="recordFailure(key: string): LoginRateLimit" />

<MemberMeta sourceHref="/source/backend/auth/loginratelimiter-ts/#L58" sourceLabel="LoginRateLimiter.ts:58" />

**Parameters**

- `key` (string)

**Returns**

- [`LoginRateLimit`](/module/backend-auth-loginratelimiter/loginratelimit)

<MemberHeading id="reset" depth="3" name="reset" sig="reset(key: string): void" />

<MemberMeta sourceHref="/source/backend/auth/loginratelimiter-ts/#L84" sourceLabel="LoginRateLimiter.ts:84" />

Call after a successful login.

**Parameters**

- `key` (string)

**Returns**

- `void`

## Static Methods

<MemberHeading
  id="loginratelimitkeys"
  depth="3"
  name="loginRateLimitKeys"
  sig="loginRateLimitKeys(
	req: Request,
	email: string,
): { accountKey: string; ipKey: string }"
/>

<MemberMeta badges="static" sourceHref="/source/backend/auth/loginratelimiter-ts/#L103" sourceLabel="LoginRateLimiter.ts:103" />

**Parameters**

- `req` (Request)
- `email` (string)

**Properties**

- `accountKey` (string)
- `ipKey` (string)

**Returns**

- `{ accountKey: string; ipKey: string }`

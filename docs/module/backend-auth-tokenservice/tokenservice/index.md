---
title: TokenService
kind: class
longname: module:backend/auth/TokenService.TokenService
description: Access tokens (a hand-rolled JWT), refresh tokens and WebSocket tickets. Sessions live only in memory, so a restart signs everyone out.
---

# TokenService

<SourceLink href="/source/backend/auth/tokenservice-ts/#L30" label="TokenService.ts:30" />

Access tokens (a hand-rolled JWT), refresh tokens and WebSocket tickets. Sessions live only in memory, so a restart signs everyone out.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new TokenService(
	__namedParameters: TokenServiceConstructor,
): TokenService"
/>

**Parameters**

- `__namedParameters` ([TokenServiceConstructor](/module/backend-auth-tokenservice/types/tokenserviceconstructor))

**Returns**

`TokenService`

---

## Methods

<MemberHeading
  id="consumewebsocketticket"
  depth="3"
  name="consumeWebSocketTicket"
  sig="consumeWebSocketTicket(
	ticket: string,
	channel: WebSocketChannel,
): Promise<AccessAuthorization>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/auth/tokenservice-ts/#L143" sourceLabel="TokenService.ts:143" />

**Parameters**

- `ticket` (string)
- `channel` (WebSocketChannel)

**Returns**

- `Promise<`[`AccessAuthorization`](/module/backend-auth-tokenservice/types/accessauthorization)`>`

<MemberHeading
  id="issuewebsocketticket"
  depth="3"
  name="issueWebSocketTicket"
  sig="issueWebSocketTicket(
	accessToken: string,
	channel: WebSocketChannel,
): Promise<WebSocketTicket>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/auth/tokenservice-ts/#L125" sourceLabel="TokenService.ts:125" />

WebSocket handshakes can't carry an `Authorization` header, hence the ticket.

**Parameters**

- `accessToken` (string)
- `channel` (WebSocketChannel)

**Returns**

- `Promise<WebSocketTicket>`

<MemberHeading
  id="onsessionrevoked"
  depth="3"
  name="onSessionRevoked"
  sig="onSessionRevoked(
	listener: (sessionId: string) => void,
): () => void"
/>

<MemberMeta sourceHref="/source/backend/auth/tokenservice-ts/#L177" sourceLabel="TokenService.ts:177" />

**Parameters**

- `listener` ((sessionId: string) => void)

**Returns**

- `() => void`

<MemberHeading id="refreshsession" depth="3" name="refreshSession" sig="refreshSession(refreshToken: string): Promise<AuthSession>" />

<MemberMeta badges="async" sourceHref="/source/backend/auth/tokenservice-ts/#L70" sourceLabel="TokenService.ts:70" />

Rotates the refresh token on every use.

**Parameters**

- `refreshToken` (string)

**Returns**

- `Promise<AuthSession>`

<MemberHeading id="revokesession" depth="3" name="revokeSession" sig="revokeSession(refreshToken: string): void" />

<MemberMeta sourceHref="/source/backend/auth/tokenservice-ts/#L106" sourceLabel="TokenService.ts:106" />

**Parameters**

- `refreshToken` (string)

**Returns**

- `void`

<MemberHeading id="sessionfor" depth="3" name="sessionFor" sig="sessionFor(user: AuthenticatedUser): AuthSession" />

<MemberMeta sourceHref="/source/backend/auth/tokenservice-ts/#L48" sourceLabel="TokenService.ts:48" />

**Parameters**

- `user` (AuthenticatedUser)

**Returns**

- `AuthSession`

<MemberHeading id="verifytoken" depth="3" name="verifyToken" sig="verifyToken(token: string): Promise<AuthenticatedUser>" />

<MemberMeta badges="async" sourceHref="/source/backend/auth/tokenservice-ts/#L62" sourceLabel="TokenService.ts:62" />

**Parameters**

- `token` (string)

**Returns**

- `Promise<AuthenticatedUser>`

---
title: AuthService
kind: class
longname: module:plugin/obSync/src/auth/AuthService.AuthService
description: "Session lifecycle: tokens in secret storage, refreshed by a timer or on a 401."
---

# AuthService

<SourceLink href="/source/plugin/obsync/src/auth/authservice-ts/#L30" label="AuthService.ts:30" />

Session lifecycle: tokens in secret storage, refreshed by a timer or on a 401.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new AuthService(
	dependencies: AuthServiceDependencies,
): AuthService"
/>

**Parameters**

- `dependencies` (AuthServiceDependencies)

**Returns**

`AuthService`

---

## Properties

<MemberHeading id="clientid" depth="3" name="clientId" sig="clientId: `${string}-${string}-${string}-${string}-${string}`" />

<MemberMeta badges="readonly" sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L42" sourceLabel="AuthService.ts:42" />

Sent to the backend so this client can recognize its own broadcast changes.

## Accessors

<MemberHeading id="user" depth="3" name="user" sig="get user(): AuthenticatedUser" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L56" sourceLabel="AuthService.ts:56" />

## Methods

<MemberHeading id="authheaders" depth="3" name="AuthHeaders" sig="AuthHeaders(): Record<string, string>" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L79" sourceLabel="AuthService.ts:79" />

**Returns**

- `Record<string, string>`

<MemberHeading id="changecolor" depth="3" name="changeColor" sig="changeColor(color: string): Promise<UserActionResult<null>>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L174" sourceLabel="AuthService.ts:174" />

Adopting the returned profile reconnects the collaboration room with the new color.

**Parameters**

- `color` (string)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<null>>`

<MemberHeading
  id="changepassword"
  depth="3"
  name="changePassword"
  sig="changePassword(
	currentPassword: string,
	newPassword: string,
): Promise<UserActionResult<null>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L128" sourceLabel="AuthService.ts:128" />

**Parameters**

- `currentPassword` (string)
- `newPassword` (string)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<null>>`

<MemberHeading id="clearsession" depth="3" name="clearSession" sig="clearSession(): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L270" sourceLabel="AuthService.ts:270" />

**Returns**

- `Promise<void>`

<MemberHeading
  id="createwebsocketticket"
  depth="3"
  name="createWebSocketTicket"
  sig="createWebSocketTicket(
	channel: WebSocketChannel,
): Promise<string>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L111" sourceLabel="AuthService.ts:111" />

Short-lived ticket that authenticates a WebSocket upgrade.

**Parameters**

- `channel` (WebSocketChannel)

**Returns**

- `Promise<string>`

<MemberHeading id="destroy" depth="3" name="destroy" sig="destroy(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L274" sourceLabel="AuthService.ts:274" />

**Returns**

- `void`

<MemberHeading id="ensureauthenticated" depth="3" name="ensureAuthenticated" sig="ensureAuthenticated(): Promise<boolean | void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L96" sourceLabel="AuthService.ts:96" />

Restores the stored session or opens the login modal.

**Returns**

- `Promise<boolean | void>`

<MemberHeading id="geneheader" depth="3" name="GeneHeader" sig="GeneHeader(savedGene: string): Record<string, string>" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L85" sourceLabel="AuthService.ts:85" />

**Parameters**

- `savedGene` (string)

**Returns**

- `Record<string, string>`

<MemberHeading id="headers" depth="3" name="headers" sig="headers(): Record<string, string>" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L71" sourceLabel="AuthService.ts:71" />

**Returns**

- `Record<string, string>`

<MemberHeading id="isadmin" depth="3" name="isAdmin" sig="isAdmin(): boolean" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L63" sourceLabel="AuthService.ts:63" />

**Returns**

- `boolean`

<MemberHeading id="isauthenticated" depth="3" name="isAuthenticated" sig="isAuthenticated(): boolean" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L60" sourceLabel="AuthService.ts:60" />

**Returns**

- `boolean`

<MemberHeading id="isreadonlyuser" depth="3" name="isReadOnlyUser" sig="isReadOnlyUser(): boolean" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L67" sourceLabel="AuthService.ts:67" />

**Returns**

- `boolean`

<MemberHeading id="logout" depth="3" name="logout" sig="logout(): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L251" sourceLabel="AuthService.ts:251" />

**Returns**

- `Promise<void>`

<MemberHeading id="prepareauthenticatedrequest" depth="3" name="prepareAuthenticatedRequest" sig="prepareAuthenticatedRequest(): Promise<boolean>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L91" sourceLabel="AuthService.ts:91" />

**Returns**

- `Promise<boolean>`

<MemberHeading id="refreshsession" depth="3" name="refreshSession" sig="refreshSession(): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L227" sourceLabel="AuthService.ts:227" />

Picks up profile changes made elsewhere, e.g. an admin changing this user's role.

**Returns**

- `Promise<void>`

<MemberHeading id="schedulesessionrefresh" depth="3" name="scheduleSessionRefresh" sig="scheduleSessionRefresh(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/authservice-ts/#L215" sourceLabel="AuthService.ts:215" />

Debounced, so several admin actions in a row cost a single request.

**Returns**

- `void`

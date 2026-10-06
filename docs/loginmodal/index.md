---
title: LoginModal
kind: class
longname: LoginModal
---

# LoginModal

<SourceLink href="/source/plugin/obsync/src/auth/loginmodal-ts/#L4" label="LoginModal.ts:4" />

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new LoginModal(
	app: App,
	submitLogin: (email: string, password: string) => Promise<boolean>,
	onFinished: (authenticated: boolean) => void,
): LoginModal"
/>

**Parameters**

- `app` (App)
- `submitLogin` ((email: string, password: string) => Promise\<boolean>)
- `onFinished` ((authenticated: boolean) => void)

**Returns**

`LoginModal`

#### Hierarchy

- `Modal`
- `LoginModal`

---

## Properties

<MemberHeading id="app" depth="3" name="app" sig="app: App" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4480" sourceLabel="obsidian.d.ts:4480" />

_Inherited from&#x20;_`app`

<MemberHeading id="containerel" depth="3" name="containerEl" sig="containerEl: HTMLElement" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4488" sourceLabel="obsidian.d.ts:4488" />

_Inherited from&#x20;_`containerEl`

<MemberHeading id="contentel" depth="3" name="contentEl" sig="contentEl: HTMLElement" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4501" sourceLabel="obsidian.d.ts:4501" />

_Inherited from&#x20;_`contentEl`

<MemberHeading id="modalel" depth="3" name="modalEl" sig="modalEl: HTMLElement" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4492" sourceLabel="obsidian.d.ts:4492" />

_Inherited from&#x20;_`modalEl`

<MemberHeading id="scope" depth="3" name="scope" sig="scope: Scope" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4484" sourceLabel="obsidian.d.ts:4484" />

_Inherited from&#x20;_`scope`

<MemberHeading id="shouldrestoreselection" depth="3" name="shouldRestoreSelection" sig="shouldRestoreSelection: boolean" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4507" sourceLabel="obsidian.d.ts:4507" />

_Inherited from&#x20;_`shouldRestoreSelection`

- **Since:** 0.9.16

<MemberHeading id="titleel" depth="3" name="titleEl" sig="titleEl: HTMLElement" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4497" sourceLabel="obsidian.d.ts:4497" />

_Inherited from&#x20;_`titleEl`

## Methods

<MemberHeading id="close" depth="3" name="close" sig="close(): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4524" sourceLabel="obsidian.d.ts:4524" />

_Inherited from&#x20;_`close`

Hide the modal.

**Returns**

- `void`

<MemberHeading id="onclose" depth="3" name="onClose" sig="onClose(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/loginmodal-ts/#L69" sourceLabel="LoginModal.ts:69" />

_Overrides&#x20;_`onClose`

**Returns**

- `void`

<MemberHeading id="onopen" depth="3" name="onOpen" sig="onOpen(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/auth/loginmodal-ts/#L26" sourceLabel="LoginModal.ts:26" />

_Overrides&#x20;_`onOpen`

**Returns**

- `void`

<MemberHeading id="open" depth="3" name="open" sig="open(): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4518" sourceLabel="obsidian.d.ts:4518" />

_Inherited from&#x20;_`open`

Show the modal on the active window. On phones, the modal will animate on screen.

**Returns**

- `void`

<MemberHeading id="setclosecallback" depth="3" name="setCloseCallback" sig="setCloseCallback(callback: () => any): this" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4547" sourceLabel="obsidian.d.ts:4547" />

_Inherited from&#x20;_`setCloseCallback`

**Parameters**

- `callback` (() => any)

**Returns**

- `this`

* **Since:** 1.10.0

<MemberHeading id="setcontent" depth="3" name="setContent" sig="setContent(content: string | DocumentFragment): this" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4541" sourceLabel="obsidian.d.ts:4541" />

_Inherited from&#x20;_`setContent`

**Parameters**

- `content` (string | DocumentFragment)

**Returns**

- `this`

<MemberHeading id="settitle" depth="3" name="setTitle" sig="setTitle(title: string): this" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4537" sourceLabel="obsidian.d.ts:4537" />

_Inherited from&#x20;_`setTitle`

**Parameters**

- `title` (string)

**Returns**

- `this`

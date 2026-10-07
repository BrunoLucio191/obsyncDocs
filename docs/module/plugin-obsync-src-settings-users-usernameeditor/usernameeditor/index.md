---
title: UserNameEditor
kind: class
longname: module:plugin/obSync/src/settings/users/UserNameEditor.UserNameEditor
description: Display-name field that saves itself, used both in Account and in the user list.
---

# UserNameEditor

<SourceLink href="/source/plugin/obsync/src/settings/users/usernameeditor-ts/#L8" label="UserNameEditor.ts:8" />

Display-name field that saves itself, used both in Account and in the user list.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new UserNameEditor(
	controller: default,
	directory: UserDirectory,
): UserNameEditor"
/>

**Parameters**

- `controller` (default)
- `directory` ([UserDirectory](/module/plugin-obsync-src-settings-users-userdirectory/userdirectory))

**Returns**

`UserNameEditor`

---

## Methods

<MemberHeading id="destroy" depth="3" name="destroy" sig="destroy(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/usernameeditor-ts/#L95" sourceLabel="UserNameEditor.ts:95" />

**Returns**

- `void`

<MemberHeading
  id="render"
  depth="3"
  name="render"
  sig="render(
	setting: Setting,
	user: AuthenticatedUser,
	label: string,
	description: string,
): void"
/>

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/usernameeditor-ts/#L20" sourceLabel="UserNameEditor.ts:20" />

**Parameters**

- `setting` (Setting)
- `user` (AuthenticatedUser)
- `label` (string)
- `description` (string)

**Returns**

- `void`

<MemberHeading
  id="schedulesave"
  depth="3"
  name="scheduleSave"
  sig="scheduleSave(
	user: AuthenticatedUser,
	value: string,
	statusEl: HTMLElement,
	inputEl: HTMLInputElement,
	onSaved?: () => void,
): void"
/>

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/usernameeditor-ts/#L41" sourceLabel="UserNameEditor.ts:41" />

The per-user generation keeps an in-flight save from overwriting a newer edit.

**Parameters**

- `user` (AuthenticatedUser)
- `value` (string)
- `statusEl` (HTMLElement)
- `inputEl` (HTMLInputElement)
- `onSaved` (() => void, optional)

**Returns**

- `void`

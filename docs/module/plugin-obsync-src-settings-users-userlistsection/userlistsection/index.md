---
title: UserListSection
kind: class
longname: module:plugin/obSync/src/settings/users/UserListSection.UserListSection
description: Admin-only account list. Controls that would lock out the last active admin are disabled.
---

# UserListSection

<SourceLink href="/source/plugin/obsync/src/settings/users/userlistsection-ts/#L19" label="UserListSection.ts:19" />

Admin-only account list. Controls that would lock out the last active admin are disabled.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new UserListSection(
	plugin: default,
	userDirectory: UserDirectory,
	nameEditor: UserNameEditor,
	refresh: () => void,
): UserListSection"
/>

**Parameters**

- `plugin` (default)
- `userDirectory` ([UserDirectory](/module/plugin-obsync-src-settings-users-userdirectory/userdirectory))
- `nameEditor` ([UserNameEditor](/module/plugin-obsync-src-settings-users-usernameeditor/usernameeditor))
- `refresh` (() => void)

**Returns**

`UserListSection`

---

## Methods

<MemberHeading id="definitions" depth="3" name="definitions" sig="definitions(): SettingDefinitionItem[]" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userlistsection-ts/#L44" sourceLabel="UserListSection.ts:44" />

Also starts the lazy load; `listGroup` stays empty until it finishes.

**Returns**

- `SettingDefinitionItem[]`

<MemberHeading id="destroy" depth="3" name="destroy" sig="destroy(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userlistsection-ts/#L117" sourceLabel="UserListSection.ts:117" />

**Returns**

- `void`

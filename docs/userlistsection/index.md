---
title: UserListSection
kind: class
longname: UserListSection
description: Admin-only account list. Controls that would lock out the last active admin are disabled.
---

# UserListSection

<SourceLink href="/source/plugin/obsync/src/settings/users/userlistsection-ts/#L15" label="UserListSection.ts:15" />

Admin-only account list. Controls that would lock out the last active admin are disabled.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new UserListSection(
	controller: ObSync,
	directory: UserDirectory,
	nameEditor: UserNameEditor,
	refresh: () => void,
): UserListSection"
/>

**Parameters**

- `controller` ([ObSync](/obsync))
- `directory` ([UserDirectory](/userdirectory))
- `nameEditor` ([UserNameEditor](/usernameeditor))
- `refresh` (() => void)

**Returns**

`UserListSection`

---

## Methods

<MemberHeading id="definitions" depth="3" name="definitions" sig="definitions(): SettingDefinitionItem[]" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userlistsection-ts/#L40" sourceLabel="UserListSection.ts:40" />

Also starts the lazy load; `listGroup` stays empty until it finishes.

**Returns**

- `SettingDefinitionItem[]`

<MemberHeading id="destroy" depth="3" name="destroy" sig="destroy(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/users/userlistsection-ts/#L123" sourceLabel="UserListSection.ts:123" />

**Returns**

- `void`

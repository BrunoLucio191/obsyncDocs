---
title: UserManagementSection
kind: class
longname: module:plugin/obSync/src/settings/UserManagementSection.UserManagementSection
description: Also lends its name editor to the Account section, so both save names the same way.
---

# UserManagementSection

<SourceLink href="/source/plugin/obsync/src/settings/usermanagementsection-ts/#L11" label="UserManagementSection.ts:11" />

Also lends its name editor to the Account section, so both save names the same way.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new UserManagementSection(
	controller: default,
	refresh: () => void,
): UserManagementSection"
/>

**Parameters**

- `controller` (default)
- `refresh` (() => void)

**Returns**

`UserManagementSection`

---

## Methods

<MemberHeading id="definitions" depth="3" name="definitions" sig="definitions(): SettingDefinitionItem[]" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/usermanagementsection-ts/#L33" sourceLabel="UserManagementSection.ts:33" />

**Returns**

- `SettingDefinitionItem[]`

<MemberHeading id="destroy" depth="3" name="destroy" sig="destroy(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/usermanagementsection-ts/#L46" sourceLabel="UserManagementSection.ts:46" />

**Returns**

- `void`

<MemberHeading
  id="rendereditablename"
  depth="3"
  name="renderEditableName"
  sig="renderEditableName(
	setting: Setting,
	user: AuthenticatedUser,
): void"
/>

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/usermanagementsection-ts/#L37" sourceLabel="UserManagementSection.ts:37" />

**Parameters**

- `setting` (Setting)
- `user` (AuthenticatedUser)

**Returns**

- `void`

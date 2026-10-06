---
title: AccountSettingsSection
kind: class
longname: AccountSettingsSection
description: Password fields get one row each, so Obsidian's layout keeps them readable at any width.
---

# AccountSettingsSection

<SourceLink href="/source/plugin/obsync/src/settings/accountsettingssection-ts/#L12" label="AccountSettingsSection.ts:12" />

Password fields get one row each, so Obsidian's layout keeps them readable at any width.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new AccountSettingsSection(
	controller: ObSync,
	users: UserManagementSection,
	refresh: () => void,
): AccountSettingsSection"
/>

**Parameters**

- `controller` ([ObSync](/obsync))
- `users` ([UserManagementSection](/usermanagementsection))
- `refresh` (() => void)

**Returns**

`AccountSettingsSection`

---

## Methods

<MemberHeading
  id="definition"
  depth="3"
  name="definition"
  sig="definition(
	currentUser: AuthenticatedUser,
): SettingDefinitionGroup"
/>

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/accountsettingssection-ts/#L32" sourceLabel="AccountSettingsSection.ts:32" />

**Parameters**

- `currentUser` ([AuthenticatedUser](/authenticateduser))

**Returns**

- `SettingDefinitionGroup`

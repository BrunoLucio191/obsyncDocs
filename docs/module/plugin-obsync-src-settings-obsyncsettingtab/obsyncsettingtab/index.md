---
title: ObSyncSettingTab
kind: class
longname: module:plugin/obSync/src/settings/ObSyncSettingTab.ObSyncSettingTab
description: Receives the other fields for settings and combina everything together
---

# ObSyncSettingTab

<SourceLink href="/source/plugin/obsync/src/settings/obsyncsettingtab-ts/#L16" label="ObSyncSettingTab.ts:16" />

Receives the other fields for settings and combina everything together

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new ObSyncSettingTab(
	app: App,
	plugin: Plugin & default,
): ObSyncSettingTab"
/>

**Parameters**

- `app` (App)
- `plugin` (Plugin & default)

**Returns**

`ObSyncSettingTab`

#### Hierarchy

- `PluginSettingTab`
- `ObSyncSettingTab`

---

## Properties

<MemberHeading id="app" depth="3" name="app" sig="app: App" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L6560" sourceLabel="obsidian.d.ts:6560" />

_Inherited from&#x20;_`app`

Reference to the app instance.

<MemberHeading id="containerel" depth="3" name="containerEl" sig="containerEl: HTMLElement" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L6566" sourceLabel="obsidian.d.ts:6566" />

_Inherited from&#x20;_`containerEl`

HTML element for the setting tab content.

<MemberHeading id="icon" depth="3" name="icon" sig="icon: string" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L6555" sourceLabel="obsidian.d.ts:6555" />

_Inherited from&#x20;_`icon`

The icon to display in the settings sidebar.

- **Since:** 1.11.0

<MemberHeading id="settingitems" depth="3" name="settingItems" sig="settingItems: SettingDefinitionItem<string>[]" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L6574" sourceLabel="obsidian.d.ts:6574" />

_Inherited from&#x20;_`settingItems`

Nested setting definitions as returned by getSettingDefinitions(). Populated by update().

- **Since:** 1.13.0

## Methods

<MemberHeading id="display" depth="3" name="display" sig="display(): void" />

<MemberMeta badges="deprecated" sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L6640" sourceLabel="obsidian.d.ts:6640" />

_Inherited from&#x20;_`display`

Override to render the tab imperatively.

Not called when [getSettingDefinitions](/module/plugin-obsync-src-settings-obsyncsettingtab/obsyncsettingtab#getsettingdefinitions) returns a non-empty array; the tab is rendered declaratively from those definitions instead. Only implement display() as a fallback for plugins that need to support Obsidian versions older than 1.13.0.

<Callout type="error">
  &#x20;Since 1.13.0. Use [getSettingDefinitions](/module/plugin-obsync-src-settings-obsyncsettingtab/obsyncsettingtab#getsettingdefinitions) instead.
</Callout>

**Returns**

- `void`

* **See:**
  - [https://docs.obsidian.md/Plugins/User+interface/Settings#Register+a+settings+tab](https://docs.obsidian.md/Plugins/User+interface/Settings#Register+a+settings+tab)

<MemberHeading id="getallconfiguration" depth="3" name="getAllConfiguration" sig="getAllConfiguration(): SettingDefinitionItem[]" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/obsyncsettingtab-ts/#L34" sourceLabel="ObSyncSettingTab.ts:34" />

**Returns**

- `SettingDefinitionItem[]`

<MemberHeading id="getcontrolvalue" depth="3" name="getControlValue" sig="getControlValue(key: string): unknown" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5165" sourceLabel="obsidian.d.ts:5165" />

_Inherited from&#x20;_`getControlValue`

Reads from `this.plugin.settings`. Override to read from a different data source.

**Parameters**

- `key` (string)

**Returns**

- `unknown`

* **Since:** 1.13.0

<MemberHeading id="getsettingdefinitions" depth="3" name="getSettingDefinitions" sig="getSettingDefinitions(): SettingDefinitionItem[]" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/obsyncsettingtab-ts/#L59" sourceLabel="ObSyncSettingTab.ts:59" />

_Overrides&#x20;_`getSettingDefinitions`

**Returns**

- `SettingDefinitionItem[]`

* **Since:** 1.13.0

<MemberHeading id="hide" depth="3" name="hide" sig="hide(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/settings/obsyncsettingtab-ts/#L63" sourceLabel="ObSyncSettingTab.ts:63" />

_Overrides&#x20;_`hide`

Hides the contents of the setting tab. Any registered components should be unloaded when the view is hidden. Override this if you need to perform additional cleanup.

**Returns**

- `void`

<MemberHeading id="refreshdomstate" depth="3" name="refreshDomState" sig="refreshDomState(): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L6627" sourceLabel="obsidian.d.ts:6627" />

_Inherited from&#x20;_`refreshDomState`

Re-evaluate every `visible` and `disabled` predicate against the current state and apply the result to the rendered DOM. Call this from a `render` callback's onChange (or any other imperative path) after mutating state that other settings' predicates depend on.

Cheap: toggles CSS state in place, no re-render. For changes that affect the structure of the definitions themselves (added or removed items), call `update()` instead.

**Returns**

- `void`

* **Since:** 1.13.0

<MemberHeading
  id="setcontrolvalue"
  depth="3"
  name="setControlValue"
  sig="setControlValue(
	key: string,
	value: unknown,
): void | Promise<void>"
/>

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5172" sourceLabel="obsidian.d.ts:5172" />

_Inherited from&#x20;_`setControlValue`

Mutates and persists `this.plugin.settings`. Override to write to a different data source.

**Parameters**

- `key` (string)
- `value` (unknown)

**Returns**

- `void | Promise<void>`

* **Since:** 1.13.0

<MemberHeading id="update" depth="3" name="update" sig="update(): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L6590" sourceLabel="obsidian.d.ts:6590" />

_Inherited from&#x20;_`update`

Stores the result of getSettingDefinitions() for rendering and search indexing. Called by addSettingTab() and by dynamic tabs when their data changes.

**Returns**

- `void`

* **Since:** 1.13.0

---
title: default
kind: class
longname: module:plugin/obSync/src/main.default
description: ObSync plugin class
---

# default

<SourceLink href="/source/plugin/obsync/src/main-ts/#L30" label="main.ts:30" />

ObSync plugin class

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new default(app: App, manifest: PluginManifest): default" />

**Parameters**

- `app` (App)
- `manifest` (PluginManifest)

**Returns**

`default`

#### Hierarchy

- `Plugin`
- `default`

---

## Properties

<MemberHeading id="app" depth="3" name="app" sig="app: App" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4906" sourceLabel="obsidian.d.ts:4906" />

_Inherited from&#x20;_`app`

- **Since:** 0.9.7

<MemberHeading id="config" depth="3" name="config" sig="config: ObSyncConfig" />

<MemberMeta sourceHref="/source/plugin/obsync/src/main-ts/#L31" sourceLabel="main.ts:31" />

<MemberHeading id="manifest" depth="3" name="manifest" sig="manifest: PluginManifest" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4911" sourceLabel="obsidian.d.ts:4911" />

_Inherited from&#x20;_`manifest`

- **Since:** 0.9.7

<MemberHeading id="settings" depth="3" name="settings" sig="settings: unknown" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4918" sourceLabel="obsidian.d.ts:4918" />

_Inherited from&#x20;_`settings`

Plugin settings. Assign loaded data here in `onload`. Declare a concrete type on your subclass to type it.

- **Since:** 1.13.0

## Methods

<MemberHeading id="addchild" depth="3" name="addChild" sig="addChild<T extends Component>(component: T): T" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L1867" sourceLabel="obsidian.d.ts:1867" />

_Inherited from&#x20;_`addChild`

Adds a child component, loading it if this component is loaded

**Type Parameters**

- `T` extends `Component`

**Parameters**

- `component` (T)

**Returns**

- `T`

* **Since:** 0.12.0

<MemberHeading id="addcommand" depth="3" name="addCommand" sig="addCommand(command: Command): Command" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4954" sourceLabel="obsidian.d.ts:4954" />

_Inherited from&#x20;_`addCommand`

Register a command globally. Registered commands will be available from the {@link [https://help.obsidian.md/Plugins/Command+palette|Command](https://help.obsidian.md/Plugins/Command+palette%7CCommand) palette}. The command id and name will be automatically prefixed with this plugin's id and name.

**Parameters**

- `command` (Command)

**Returns**

- `Command`

* **Since:** 0.9.7

<MemberHeading
  id="addribbonicon"
  depth="3"
  name="addRibbonIcon"
  sig="addRibbonIcon(
	icon: string,
	title: string,
	callback: (evt: MouseEvent) => any,
): HTMLElement"
/>

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4937" sourceLabel="obsidian.d.ts:4937" />

_Inherited from&#x20;_`addRibbonIcon`

Adds a ribbon icon to the left bar.

**Parameters**

- `icon` (string) — The icon name to be used. See `addIcon`
- `title` (string) — The title to be displayed in the tooltip.
- `callback` ((evt: MouseEvent) => any) — The `click` callback.

**Returns**

- `HTMLElement`

* **Since:** 0.9.7

<MemberHeading id="addsettingtab" depth="3" name="addSettingTab" sig="addSettingTab(settingTab: PluginSettingTab): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4968" sourceLabel="obsidian.d.ts:4968" />

_Inherited from&#x20;_`addSettingTab`

Register a settings tab, which allows users to change settings.

**Parameters**

- `settingTab` (PluginSettingTab)

**Returns**

- `void`

* **Since:** 0.9.7
* **See:**
  - [https://docs.obsidian.md/Plugins/User+interface/Settings#Register+a+settings+tab](https://docs.obsidian.md/Plugins/User+interface/Settings#Register+a+settings+tab)

<MemberHeading id="addstatusbaritem" depth="3" name="addStatusBarItem" sig="addStatusBarItem(): HTMLElement" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4946" sourceLabel="obsidian.d.ts:4946" />

_Inherited from&#x20;_`addStatusBarItem`

Adds a status bar item to the bottom of the app. Not available on mobile.

**Returns**

- `HTMLElement` — HTMLElement - element to modify.

* **Since:** 0.9.7
* **See:**
  - [https://docs.obsidian.md/Plugins/User+interface/Status+bar](https://docs.obsidian.md/Plugins/User+interface/Status+bar)

<MemberHeading id="changecolor" depth="3" name="changeColor" sig="changeColor(color: string): Promise<UserActionResult<null>>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L176" sourceLabel="main.ts:176" />

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

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L169" sourceLabel="main.ts:169" />

**Parameters**

- `currentPassword` (string)
- `newPassword` (string)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<null>>`

<MemberHeading
  id="createuser"
  depth="3"
  name="createUser"
  sig="createUser(
	input: { email: string; name: string; password: string; role: UserRole },
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L126" sourceLabel="main.ts:126" />

**Parameters**

- `input` ({ email: string; name: string; password: string; role: UserRole })

**Properties**

- `email` (string)
- `name` (string)
- `password` (string)
- `role` (UserRole)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading
  id="deleteuser"
  depth="3"
  name="deleteUser"
  sig="deleteUser(
	userId: number,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L149" sourceLabel="main.ts:149" />

**Parameters**

- `userId` (number)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading id="ensurelogin" depth="3" name="ensureLogin" sig="ensureLogin(): Promise<boolean>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L97" sourceLabel="main.ts:97" />

**Returns**

- `Promise<boolean>`

<MemberHeading id="isauthenticated" depth="3" name="isAuthenticated" sig="isAuthenticated(): boolean" />

<MemberMeta sourceHref="/source/plugin/obsync/src/main-ts/#L118" sourceLabel="main.ts:118" />

**Returns**

- `boolean`

<MemberHeading id="listusers" depth="3" name="listUsers" sig="listUsers(): Promise<UserActionResult<AuthenticatedUser[]>>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L122" sourceLabel="main.ts:122" />

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser[]>>`

<MemberHeading id="load" depth="3" name="load" sig="load(): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L1841" sourceLabel="obsidian.d.ts:1841" />

_Inherited from&#x20;_`load`

Load this component and its children

**Returns**

- `void`

* **Since:** 0.9.7

<MemberHeading id="loaddata" depth="3" name="loadData" sig="loadData(): Promise<any>" />

<MemberMeta badges="async" sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5055" sourceLabel="obsidian.d.ts:5055" />

_Inherited from&#x20;_`loadData`

Load settings data from disk. Data is stored in `data.json` in the plugin folder.

**Returns**

- `Promise<any>`

* **Since:** 0.9.7
* **See:**
  - [https://docs.obsidian.md/Plugins/User+interface/Settings](https://docs.obsidian.md/Plugins/User+interface/Settings)

<MemberHeading id="logout" depth="3" name="logout" sig="logout(): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L106" sourceLabel="main.ts:106" />

Opens the login right away, so another account can sign in.

**Returns**

- `Promise<void>`

<MemberHeading id="onexternalsettingschange" depth="3" name="onExternalSettingsChange" sig="onExternalSettingsChange(): any" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5084" sourceLabel="obsidian.d.ts:5084" />

_Inherited from&#x20;_`onExternalSettingsChange`

Called when the `data.json` file is modified on disk externally from Obsidian. This usually means that a Sync service or external program has modified the plugin settings.

Implement this method to reload plugin settings when they have changed externally.

**Returns**

- `any`

* **Since:** 1.5.7

<MemberHeading id="onload" depth="3" name="onload" sig="onload(): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L47" sourceLabel="main.ts:47" />

_Overrides&#x20;_`onload`

**Returns**

- `Promise<void>`

* **Since:** 0.9.7

<MemberHeading id="onunload" depth="3" name="onunload" sig="onunload(): void" />

<MemberMeta sourceHref="/source/plugin/obsync/src/main-ts/#L67" sourceLabel="main.ts:67" />

_Overrides&#x20;_`onunload`

Override this to unload your component

**Returns**

- `void`

* **Since:** 0.9.7

<MemberHeading id="onuserenable" depth="3" name="onUserEnable" sig="onUserEnable(): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5072" sourceLabel="obsidian.d.ts:5072" />

_Inherited from&#x20;_`onUserEnable`

Perform any initial setup code. The user has explicitly interacted with the plugin so its safe to engage with the user. If your plugin registers a custom view, you can open it here.

**Returns**

- `void`

* **Since:** 1.7.2

<MemberHeading id="openlogin" depth="3" name="openLogin" sig="openLogin(): Promise<boolean>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L76" sourceLabel="main.ts:76" />

**Returns**

- `Promise<boolean>`

<MemberHeading id="register" depth="3" name="register" sig="register(cb: () => any): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L1879" sourceLabel="obsidian.d.ts:1879" />

_Inherited from&#x20;_`register`

Registers a callback to be called when unloading

**Parameters**

- `cb` (() => any)

**Returns**

- `void`

* **Since:** 0.9.7

<MemberHeading
  id="registerbasesview"
  depth="3"
  name="registerBasesView"
  sig="registerBasesView(
	viewId: string,
	registration: BasesViewRegistration,
): boolean"
/>

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5008" sourceLabel="obsidian.d.ts:5008" />

_Inherited from&#x20;_`registerBasesView`

Register a Base view handler that can be used to render data from property queries.

**Parameters**

- `viewId` (string)
- `registration` (BasesViewRegistration)

**Returns**

- `boolean` — false if bases are not enabled in this vault.

* **Since:** 1.10.0

<MemberHeading
  id="registerclihandler"
  depth="3"
  name="registerCliHandler"
  sig="registerCliHandler(
	command: string,
	description: string,
	flags: CliFlags,
	handler: CliHandler,
): void"
/>

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5047" sourceLabel="obsidian.d.ts:5047" />

_Inherited from&#x20;_`registerCliHandler`

Register a CLI handler to handle a command from the CLI. Command IDs must be globally unique. Attempting to register a command that is already registered will throw an Error.

Use the format `<plugin-id>` for your default command, and `<plugin-id>:<action>` for sub-commands and actions.

**Parameters**

- `command` (string) — The command ID that will be used. Use alphanumeric characters without spaces.
- `description` (string) — The description text to provide in the help command, and in auto-completion prompts.
- `flags` (CliFlags) — Command line flags that can be passed in.
- `handler` (CliHandler) — The callback handler to handle a CLI invocation.

**Returns**

- `void`

* **Since:** 1.12.2

<MemberHeading id="registerdomevent" depth="3" name="registerDomEvent" sig="registerDomEvent" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L1891" sourceLabel="obsidian.d.ts:1891" />

_Inherited from&#x20;_`registerDomEvent`

Registers a DOM event to be detached when unloading

- **Since:** 0.14.8

<Signature
  code="registerDomEvent<
	K extends keyof WindowEventMap,
>(
	el: Window,
	type: K,
	callback: (this: HTMLElement, ev: WindowEventMap[K]) => any,
	options?: boolean | AddEventListenerOptions,
): void"
/>

**Type Parameters**

- `K` extends `keyof WindowEventMap`

**Parameters**

- `el` (Window)
- `type` (K)
- `callback` ((this: HTMLElement, ev: WindowEventMap\[K]) => any)
- `options` (boolean | AddEventListenerOptions, optional)

**Returns**

- `void`

<Signature
  code="registerDomEvent<
	K extends keyof DocumentEventMap,
>(
	el: Document,
	type: K,
	callback: (this: HTMLElement, ev: DocumentEventMap[K]) => any,
	options?: boolean | AddEventListenerOptions,
): void"
/>

Registers a DOM event to be detached when unloading

**Type Parameters**

- `K` extends `keyof DocumentEventMap`

**Parameters**

- `el` (Document)
- `type` (K)
- `callback` ((this: HTMLElement, ev: DocumentEventMap\[K]) => any)
- `options` (boolean | AddEventListenerOptions, optional)

**Returns**

- `void`

<Signature
  code="registerDomEvent<
	K extends keyof HTMLElementEventMap,
>(
	el: HTMLElement,
	type: K,
	callback: (this: HTMLElement, ev: HTMLElementEventMap[K]) => any,
	options?: boolean | AddEventListenerOptions,
): void"
/>

Registers a DOM event to be detached when unloading

**Type Parameters**

- `K` extends `keyof HTMLElementEventMap`

**Parameters**

- `el` (HTMLElement)
- `type` (K)
- `callback` ((this: HTMLElement, ev: HTMLElementEventMap\[K]) => any)
- `options` (boolean | AddEventListenerOptions, optional)

**Returns**

- `void`

<MemberHeading id="registereditorextension" depth="3" name="registerEditorExtension" sig="registerEditorExtension(extension: Extension): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5018" sourceLabel="obsidian.d.ts:5018" />

_Inherited from&#x20;_`registerEditorExtension`

Registers a CodeMirror 6 extension. To reconfigure cm6 extensions for a plugin on the fly, an array should be passed in, and modified dynamically. Once this array is modified, calling `Workspace.updateOptions` will apply the changes.

**Parameters**

- `extension` (Extension) — must be a CodeMirror 6 `Extension`, or an array of Extensions.

**Returns**

- `void`

* **Since:** 0.12.8

<MemberHeading id="registereditorsuggest" depth="3" name="registerEditorSuggest" sig="registerEditorSuggest(editorSuggest: EditorSuggest<any>): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5033" sourceLabel="obsidian.d.ts:5033" />

_Inherited from&#x20;_`registerEditorSuggest`

Register an EditorSuggest which can provide live suggestions while the user is typing.

**Parameters**

- `editorSuggest` (EditorSuggest\<any>)

**Returns**

- `void`

* **Since:** 0.12.7

<MemberHeading id="registerevent" depth="3" name="registerEvent" sig="registerEvent(eventRef: EventRef): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L1885" sourceLabel="obsidian.d.ts:1885" />

_Inherited from&#x20;_`registerEvent`

Registers an event to be detached when unloading

**Parameters**

- `eventRef` (EventRef)

**Returns**

- `void`

* **Since:** 0.9.7

<MemberHeading id="registerextensions" depth="3" name="registerExtensions" sig="registerExtensions(extensions: string[], viewType: string): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4984" sourceLabel="obsidian.d.ts:4984" />

_Inherited from&#x20;_`registerExtensions`

**Parameters**

- `extensions` (string\[])
- `viewType` (string)

**Returns**

- `void`

* **Since:** 0.9.7

<MemberHeading id="registerhoverlinksource" depth="3" name="registerHoverLinkSource" sig="registerHoverLinkSource(id: string, info: HoverLinkSource): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4979" sourceLabel="obsidian.d.ts:4979" />

_Inherited from&#x20;_`registerHoverLinkSource`

Registers a view with the 'Page preview' core plugin as an emitter of the 'hover-link' event.

**Parameters**

- `id` (string)
- `info` (HoverLinkSource)

**Returns**

- `void`

* **Since:** 1.1.0

<MemberHeading id="registerinterval" depth="3" name="registerInterval" sig="registerInterval(id: number): number" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L1911" sourceLabel="obsidian.d.ts:1911" />

_Inherited from&#x20;_`registerInterval`

Registers an interval (from setInterval) to be cancelled when unloading Use `window.setInterval` instead of `setInterval` to avoid TypeScript confusing between NodeJS vs Browser API

**Parameters**

- `id` (number)

**Returns**

- `number`

* **Since:** 0.13.8

<MemberHeading
  id="registermarkdowncodeblockprocessor"
  depth="3"
  name="registerMarkdownCodeBlockProcessor"
  sig="registerMarkdownCodeBlockProcessor(
	language: string,
	handler: (source: string, el: HTMLElement, ctx: MarkdownPostProcessorContext) => void | Promise<any>,
	sortOrder?: number,
): MarkdownPostProcessor"
/>

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5000" sourceLabel="obsidian.d.ts:5000" />

_Inherited from&#x20;_`registerMarkdownCodeBlockProcessor`

Register a special post processor that handles fenced code given a language and a handler. This special post processor takes care of removing the `<pre><code>` and create a `<div>` that will be passed to the handler, and is expected to be filled with custom elements.

**Parameters**

- `language` (string)
- `handler` ((source: string, el: HTMLElement, ctx: MarkdownPostProcessorContext) => void | Promise\<any>)
- `sortOrder` (number, optional)

**Returns**

- `MarkdownPostProcessor`

* **Since:** 0.9.7
* **See:**
  - [https://docs.obsidian.md/Plugins/Editor/Markdown+post+processing#Post-process+Markdown+code+blocks](https://docs.obsidian.md/Plugins/Editor/Markdown+post+processing#Post-process+Markdown+code+blocks)

<MemberHeading
  id="registermarkdownpostprocessor"
  depth="3"
  name="registerMarkdownPostProcessor"
  sig="registerMarkdownPostProcessor(
	postProcessor: MarkdownPostProcessor,
	sortOrder?: number,
): MarkdownPostProcessor"
/>

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4991" sourceLabel="obsidian.d.ts:4991" />

_Inherited from&#x20;_`registerMarkdownPostProcessor`

Registers a post processor, to change how the document looks in reading mode.

**Parameters**

- `postProcessor` (MarkdownPostProcessor)
- `sortOrder` (number, optional)

**Returns**

- `MarkdownPostProcessor`

* **Since:** 0.9.7
* **See:**
  - [https://docs.obsidian.md/Plugins/Editor/Markdown+post+processing](https://docs.obsidian.md/Plugins/Editor/Markdown+post+processing)

<MemberHeading
  id="registerobsidianprotocolhandler"
  depth="3"
  name="registerObsidianProtocolHandler"
  sig="registerObsidianProtocolHandler(
	action: string,
	handler: ObsidianProtocolHandler,
): void"
/>

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5027" sourceLabel="obsidian.d.ts:5027" />

_Inherited from&#x20;_`registerObsidianProtocolHandler`

Register a handler for obsidian:// URLs.

**Parameters**

- `action` (string) — the action string. For example, 'open' corresponds to `obsidian://open`.
- `handler` (ObsidianProtocolHandler) — the callback to trigger. A key-value pair that is decoded from the query will be passed in. For example, `obsidian://open?key=value` would generate `{'action': 'open', 'key': 'value'}`.

**Returns**

- `void`

* **Since:** 0.11.0

<MemberHeading id="registerview" depth="3" name="registerView" sig="registerView(type: string, viewCreator: ViewCreator): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4973" sourceLabel="obsidian.d.ts:4973" />

_Inherited from&#x20;_`registerView`

**Parameters**

- `type` (string)
- `viewCreator` (ViewCreator)

**Returns**

- `void`

* **Since:** 0.9.7

<MemberHeading id="removechild" depth="3" name="removeChild" sig="removeChild<T extends Component>(component: T): T" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L1873" sourceLabel="obsidian.d.ts:1873" />

_Inherited from&#x20;_`removeChild`

Removes a child component, unloading it

**Type Parameters**

- `T` extends `Component`

**Parameters**

- `component` (T)

**Returns**

- `T`

* **Since:** 0.12.0

<MemberHeading id="removecommand" depth="3" name="removeCommand" sig="removeCommand(commandId: string): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L4961" sourceLabel="obsidian.d.ts:4961" />

_Inherited from&#x20;_`removeCommand`

Manually remove a command from the list of global commands. This should not be needed unless your plugin registers commands dynamically.

**Parameters**

- `commandId` (string)

**Returns**

- `void`

* **Since:** 1.7.2

<MemberHeading
  id="resetuserpassword"
  depth="3"
  name="resetUserPassword"
  sig="resetUserPassword(
	userId: number,
	newPassword: string,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L162" sourceLabel="main.ts:162" />

**Parameters**

- `userId` (number)
- `newPassword` (string)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading id="savedata" depth="3" name="saveData" sig="saveData(data: any): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L5063" sourceLabel="obsidian.d.ts:5063" />

_Inherited from&#x20;_`saveData`

Write settings data to disk. Data is stored in `data.json` in the plugin folder.

**Parameters**

- `data` (any)

**Returns**

- `Promise<void>`

* **Since:** 0.9.7
* **See:**
  - [https://docs.obsidian.md/Plugins/User+interface/Settings](https://docs.obsidian.md/Plugins/User+interface/Settings)

<MemberHeading id="setbackendurl" depth="3" name="setBackendUrl" sig="setBackendUrl(url: string): Promise<UserActionResult<null>>" />

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L180" sourceLabel="main.ts:180" />

**Parameters**

- `url` (string)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<null>>`

<MemberHeading id="unload" depth="3" name="unload" sig="unload(): void" />

<MemberMeta sourceHref="/source/node-modules/obsidian/obsidian-d-ts/#L1854" sourceLabel="obsidian.d.ts:1854" />

_Inherited from&#x20;_`unload`

Unload this component and its children

**Returns**

- `void`

* **Since:** 0.9.7

<MemberHeading
  id="updateusername"
  depth="3"
  name="updateUserName"
  sig="updateUserName(
	userId: number,
	name: string,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L155" sourceLabel="main.ts:155" />

**Parameters**

- `userId` (number)
- `name` (string)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading
  id="updateuserrole"
  depth="3"
  name="updateUserRole"
  sig="updateUserRole(
	userId: number,
	role: UserRole,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L135" sourceLabel="main.ts:135" />

**Parameters**

- `userId` (number)
- `role` (UserRole)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

<MemberHeading
  id="updateuserstatus"
  depth="3"
  name="updateUserStatus"
  sig="updateUserStatus(
	userId: number,
	active: boolean,
): Promise<UserActionResult<AuthenticatedUser>>"
/>

<MemberMeta badges="async" sourceHref="/source/plugin/obsync/src/main-ts/#L142" sourceLabel="main.ts:142" />

**Parameters**

- `userId` (number)
- `active` (boolean)

**Returns**

- `Promise<`[`UserActionResult`](/module/plugin-obsync-src-auth-auth/types/useractionresult)`<AuthenticatedUser>>`

## Static Properties

<MemberHeading id="obsyncapp" depth="3" name="obsyncApp" sig="obsyncApp: default" />

<MemberMeta badges="static" sourceHref="/source/plugin/obsync/src/main-ts/#L32" sourceLabel="main.ts:32" />

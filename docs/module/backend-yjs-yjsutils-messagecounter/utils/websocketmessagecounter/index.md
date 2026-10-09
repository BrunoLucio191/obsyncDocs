---
title: WebSocketMessageCounter
kind: interface
longname: module:backend/yjs/yjsUtils/MessageCounter.utils.WebSocketMessageCounter
---

# WebSocketMessageCounter

<Signature
  code="interface WebSocketMessageCounter<K, V> extends Map<K, V> {
	[toStringTag]: string;
	size: number;
	[iterator](): MapIterator<[K, V]>;
	biggest(): WebSocket;
	clear(): void;
	decrement(key: K): void;
	delete(key: K): boolean;
	entries(): MapIterator<[K, V]>;
	forEach(callbackfn: (value: V, key: K, map: Map<K, V>) => void, thisArg?: any): void;
	get(key: K): V;
	has(key: K): boolean;
	increment(key: K): void;
	keys(): MapIterator<K>;
	set(key: K, value: V): this;
	values(): MapIterator<V>;
}"
/>

<SourceLink href="/source/backend/yjs/yjsutils/messagecounter-utils-ts/#L3" label="MessageCounter.utils.ts:3" />

**Type Parameters**

- `K`
- `V`

#### Hierarchy

- `Map<K, V>`
- `WebSocketMessageCounter`

---

## Properties

<MemberHeading id="tostringtag" depth="3" name="[toStringTag]" sig="[toStringTag]: string" />

<MemberMeta badges="readonly" sourceHref="/source/node-modules/typescript/lib/lib-es2015-symbol-wellknown-d-ts/#L137" sourceLabel="lib.es2015.symbol.wellknown.d.ts:137" />

_Inherited from&#x20;_`[toStringTag]`

<MemberHeading id="size" depth="3" name="size" sig="size: number" />

<MemberMeta badges="readonly" sourceHref="/source/node-modules/typescript/lib/lib-es2015-collection-d-ts/#L45" sourceLabel="lib.es2015.collection.d.ts:45" />

_Inherited from&#x20;_`size`

**Returns**

- the number of elements in the Map.

## Methods

<MemberHeading id="iterator" depth="3" name="[iterator]" sig="[iterator](): MapIterator<[K, V]>" />

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-iterable-d-ts/#L143" sourceLabel="lib.es2015.iterable.d.ts:143" />

_Inherited from&#x20;_`[iterator]`

Returns an iterable of entries in the map.

**Returns**

- `MapIterator<[K, V]>`

<MemberHeading id="biggest" depth="3" name="biggest" sig="biggest(): WebSocket" />

<MemberMeta sourceHref="/source/backend/yjs/yjsutils/messagecounter-utils-ts/#L6" sourceLabel="MessageCounter.utils.ts:6" />

**Returns**

- `WebSocket`

<MemberHeading id="clear" depth="3" name="clear" sig="clear(): void" />

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-collection-d-ts/#L20" sourceLabel="lib.es2015.collection.d.ts:20" />

_Inherited from&#x20;_`clear`

**Returns**

- `void`

<MemberHeading id="decrement" depth="3" name="decrement" sig="decrement(key: K): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsutils/messagecounter-utils-ts/#L5" sourceLabel="MessageCounter.utils.ts:5" />

**Parameters**

- `key` (K)

**Returns**

- `void`

<MemberHeading id="delete" depth="3" name="delete" sig="delete(key: K): boolean" />

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-collection-d-ts/#L24" sourceLabel="lib.es2015.collection.d.ts:24" />

_Inherited from&#x20;_`delete`

**Parameters**

- `key` (K)

**Returns**

- `boolean` — true if an element in the Map existed and has been removed, or false if the element does not exist.

<MemberHeading id="entries" depth="3" name="entries" sig="entries(): MapIterator<[K, V]>" />

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-iterable-d-ts/#L148" sourceLabel="lib.es2015.iterable.d.ts:148" />

_Inherited from&#x20;_`entries`

Returns an iterable of key, value pairs for every entry in the map.

**Returns**

- `MapIterator<[K, V]>`

<MemberHeading
  id="foreach"
  depth="3"
  name="forEach"
  sig="forEach(
	callbackfn: (value: V, key: K, map: Map<K, V>) => void,
	thisArg?: any,
): void"
/>

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-collection-d-ts/#L28" sourceLabel="lib.es2015.collection.d.ts:28" />

_Inherited from&#x20;_`forEach`

Executes a provided function once per each key/value pair in the Map, in insertion order.

**Parameters**

- `callbackfn` ((value: V, key: K, map: Map\<K, V>) => void)
- `thisArg` (any, optional)

**Returns**

- `void`

<MemberHeading id="get" depth="3" name="get" sig="get(key: K): V" />

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-collection-d-ts/#L33" sourceLabel="lib.es2015.collection.d.ts:33" />

_Inherited from&#x20;_`get`

Returns a specified element from the Map object. If the value that is associated to the provided key is an object, then you will get a reference to that object and any change made to that object will effectively modify it inside the Map.

**Parameters**

- `key` (K)

**Returns**

- `V` — Returns the element associated with the specified key. If no element is associated with the specified key, undefined is returned.

<MemberHeading id="has" depth="3" name="has" sig="has(key: K): boolean" />

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-collection-d-ts/#L37" sourceLabel="lib.es2015.collection.d.ts:37" />

_Inherited from&#x20;_`has`

**Parameters**

- `key` (K)

**Returns**

- `boolean` — boolean indicating whether an element with the specified key exists or not.

<MemberHeading id="increment" depth="3" name="increment" sig="increment(key: K): void" />

<MemberMeta sourceHref="/source/backend/yjs/yjsutils/messagecounter-utils-ts/#L4" sourceLabel="MessageCounter.utils.ts:4" />

**Parameters**

- `key` (K)

**Returns**

- `void`

<MemberHeading id="keys" depth="3" name="keys" sig="keys(): MapIterator<K>" />

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-iterable-d-ts/#L153" sourceLabel="lib.es2015.iterable.d.ts:153" />

_Inherited from&#x20;_`keys`

Returns an iterable of keys in the map

**Returns**

- `MapIterator<K>`

<MemberHeading id="set" depth="3" name="set" sig="set(key: K, value: V): this" />

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-collection-d-ts/#L41" sourceLabel="lib.es2015.collection.d.ts:41" />

_Inherited from&#x20;_`set`

Adds a new element with a specified key and value to the Map. If an element with the same key already exists, the element will be updated.

**Parameters**

- `key` (K)
- `value` (V)

**Returns**

- `this`

<MemberHeading id="values" depth="3" name="values" sig="values(): MapIterator<V>" />

<MemberMeta sourceHref="/source/node-modules/typescript/lib/lib-es2015-iterable-d-ts/#L158" sourceLabel="lib.es2015.iterable.d.ts:158" />

_Inherited from&#x20;_`values`

Returns an iterable of values in the map

**Returns**

- `MapIterator<V>`

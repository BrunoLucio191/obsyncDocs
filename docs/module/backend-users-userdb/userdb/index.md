---
title: UserDB
kind: class
longname: module:backend/users/UserDB.UserDB
description: responsible for all the estructural of the sqlite database
---

# UserDB

<SourceLink href="/source/backend/users/userdb-ts/#L17" label="UserDB.ts:17" />

responsible for all the estructural of the sqlite database

---

## Constructors

<MemberHeading id="constructor" depth="3" name="constructor" sig="new UserDB(path: string): UserDB" />

**Parameters**

- `path` (string)

**Returns**

`UserDB`

#### Hierarchy

- `DatabaseSync`
- `UserDB`

---

## Properties

<MemberHeading id="isopen" depth="3" name="isOpen" sig="isOpen: boolean" />

<MemberMeta badges="readonly" sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L417" sourceLabel="sqlite.d.ts:417" />

_Inherited from&#x20;_`isOpen`

Whether the database is currently open or not.

- **Since:** v22.15.0

<MemberHeading id="istransaction" depth="3" name="isTransaction" sig="isTransaction: boolean" />

<MemberMeta badges="readonly" sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L423" sourceLabel="sqlite.d.ts:423" />

_Inherited from&#x20;_`isTransaction`

Whether the database is currently within a transaction. This method is a wrapper around [`sqlite3_get_autocommit()`](https://sqlite.org/c3ref/get_autocommit.html).

- **Since:** v24.0.0

<MemberHeading id="limits" depth="3" name="limits" sig="limits: DatabaseLimits" />

<MemberMeta badges="readonly" sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L448" sourceLabel="sqlite.d.ts:448" />

_Inherited from&#x20;_`limits`

An object for getting and setting SQLite database limits at runtime. Each property corresponds to an SQLite limit and can be read or written.

```js
const db = new DatabaseSync(':memory:');

// Read current limit
console.log(db.limits.length);

// Set a new limit
db.limits.sqlLength = 100000;

// Reset a limit to its compile-time maximum
db.limits.sqlLength = Infinity;
```

Available properties: `length`, `sqlLength`, `column`, `exprDepth`, `compoundSelect`, `vdbeOp`, `functionArg`, `attach`, `likePatternLength`, `variableNumber`, `triggerDepth`.

Setting a property to `Infinity` resets the limit to its compile-time maximum value.

- **Since:** v25.8.0

## Methods

<MemberHeading id="dispose" depth="3" name="[dispose]" sig="[dispose](): void" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L650" sourceLabel="sqlite.d.ts:650" />

_Inherited from&#x20;_`[dispose]`

Closes the database connection. If the database connection is already closed then this is a no-op.

**Returns**

- `void`

* **Since:** v22.15.0

<MemberHeading id="aggregate" depth="3" name="aggregate" sig="aggregate" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L289" sourceLabel="sqlite.d.ts:289" />

_Inherited from&#x20;_`aggregate`

Registers a new aggregate function with the SQLite database. This method is a wrapper around [`sqlite3_create_window_function()`](https://www.sqlite.org/c3ref/create_function.html).

When used as a window function, the `result` function will be called multiple times.

```js
import { DatabaseSync } from 'node:sqlite';

const db = new DatabaseSync(':memory:');
db.exec(`
  CREATE TABLE t3(x, y);
  INSERT INTO t3 VALUES ('a', 4),
                        ('b', 5),
                        ('c', 3),
                        ('d', 8),
                        ('e', 1);
`);

db.aggregate('sumint', {
  start: 0,
  step: (acc, value) => acc + value,
});

db.prepare('SELECT sumint(y) as total FROM t3').get(); // { total: 21 }
```

- **Since:** v24.0.0

<Signature code="aggregate(name: string, options: AggregateOptions): void" />

**Parameters**

- `name` (string) — The name of the SQLite function to create.
- `options` (AggregateOptions) — Function configuration settings.

**Returns**

- `void`

<Signature
  code="aggregate<
	T extends SQLInputValue,
>(
	name: string,
	options: AggregateOptions<T>,
): void"
/>

Registers a new aggregate function with the SQLite database. This method is a wrapper around [`sqlite3_create_window_function()`](https://www.sqlite.org/c3ref/create_function.html).

When used as a window function, the `result` function will be called multiple times.

```js
import { DatabaseSync } from 'node:sqlite';

const db = new DatabaseSync(':memory:');
db.exec(`
  CREATE TABLE t3(x, y);
  INSERT INTO t3 VALUES ('a', 4),
                        ('b', 5),
                        ('c', 3),
                        ('d', 8),
                        ('e', 1);
`);

db.aggregate('sumint', {
  start: 0,
  step: (acc, value) => acc + value,
});

db.prepare('SELECT sumint(y) as total FROM t3').get(); // { total: 21 }
```

**Type Parameters**

- `T` extends `SQLInputValue`

**Parameters**

- `name` (string) — The name of the SQLite function to create.
- `options` (AggregateOptions\<T>) — Function configuration settings.

**Returns**

- `void`

<MemberHeading
  id="applychangeset"
  depth="3"
  name="applyChangeset"
  sig="applyChangeset(
	changeset: Uint8Array,
	options?: ApplyChangesetOptions,
): boolean"
/>

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L644" sourceLabel="sqlite.d.ts:644" />

_Inherited from&#x20;_`applyChangeset`

An exception is thrown if the database is not open. This method is a wrapper around [`sqlite3changeset_apply()`](https://www.sqlite.org/session/sqlite3changeset_apply.html).

```js
import { DatabaseSync } from 'node:sqlite';

const sourceDb = new DatabaseSync(':memory:');
const targetDb = new DatabaseSync(':memory:');

sourceDb.exec('CREATE TABLE data(key INTEGER PRIMARY KEY, value TEXT)');
targetDb.exec('CREATE TABLE data(key INTEGER PRIMARY KEY, value TEXT)');

const session = sourceDb.createSession();

const insert = sourceDb.prepare('INSERT INTO data (key, value) VALUES (?, ?)');
insert.run(1, 'hello');
insert.run(2, 'world');

const changeset = session.changeset();
targetDb.applyChangeset(changeset);
// Now that the changeset has been applied, targetDb contains the same data as sourceDb.
```

**Parameters**

- `changeset` (Uint8Array) — A binary changeset or patchset.
- `options` (ApplyChangesetOptions, optional) — The configuration options for how the changes will be applied.

**Returns**

- `boolean` — Whether the changeset was applied successfully without being aborted.

* **Since:** v22.12.0

<MemberHeading id="close" depth="3" name="close" sig="close(): void" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L296" sourceLabel="sqlite.d.ts:296" />

_Inherited from&#x20;_`close`

Closes the database connection. An exception is thrown if the database is not open. This method is a wrapper around [`sqlite3_close_v2()`](https://www.sqlite.org/c3ref/close.html).

**Returns**

- `void`

* **Since:** v22.5.0

<MemberHeading id="createsession" depth="3" name="createSession" sig="createSession(options?: CreateSessionOptions): Session" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L614" sourceLabel="sqlite.d.ts:614" />

_Inherited from&#x20;_`createSession`

Creates and attaches a session to the database. This method is a wrapper around [`sqlite3session_create()`](https://www.sqlite.org/session/sqlite3session_create.html) and [`sqlite3session_attach()`](https://www.sqlite.org/session/sqlite3session_attach.html).

**Parameters**

- `options` (CreateSessionOptions, optional) — The configuration options for the session.

**Returns**

- `Session` — A session handle.

* **Since:** v22.12.0

<MemberHeading id="createtagstore" depth="3" name="createTagStore" sig="createTagStore(maxSize?: number): SQLTagStore" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L605" sourceLabel="sqlite.d.ts:605" />

_Inherited from&#x20;_`createTagStore`

Creates a new `SQLTagStore`, which is a Least Recently Used (LRU) cache for storing prepared statements. This allows for the efficient reuse of prepared statements by tagging them with a unique identifier.

When a tagged SQL literal is executed, the `SQLTagStore` checks if a prepared statement for the corresponding SQL query string already exists in the cache. If it does, the cached statement is used. If not, a new prepared statement is created, executed, and then stored in the cache for future use. This mechanism helps to avoid the overhead of repeatedly parsing and preparing the same SQL statements.

Tagged statements bind the placeholder values from the template literal as parameters to the underlying prepared statement. For example:

```js
sqlTagStore.get`SELECT ${value}`;
```

is equivalent to:

```js
db.prepare('SELECT ?').get(value);
```

However, in the first example, the tag store will cache the underlying prepared statement for future use.

> **Note:** The `${value}` syntax in tagged statements _binds_ a parameter to the prepared statement. This differs from its behavior in _untagged_ template literals, where it performs string interpolation.
>
> ```js
> // This a safe example of binding a parameter to a tagged statement.
> sqlTagStore.run`INSERT INTO t1 (id) VALUES (${id})`;
>
> // This is an *unsafe* example of an untagged template string.
> // `id` is interpolated into the query text as a string.
> // This can lead to SQL injection and data corruption.
> db.run(`INSERT INTO t1 (id) VALUES (${id})`);
> ```

The tag store will match a statement from the cache if the query strings (including the positions of any bound placeholders) are identical.

```js
// The following statements will match in the cache:
sqlTagStore.get`SELECT * FROM t1 WHERE id = ${id} AND active = 1`;
sqlTagStore.get`SELECT * FROM t1 WHERE id = ${12345} AND active = 1`;

// The following statements will not match, as the query strings
// and bound placeholders differ:
sqlTagStore.get`SELECT * FROM t1 WHERE id = ${id} AND active = 1`;
sqlTagStore.get`SELECT * FROM t1 WHERE id = 12345 AND active = 1`;

// The following statements will not match, as matches are case-sensitive:
sqlTagStore.get`SELECT * FROM t1 WHERE id = ${id} AND active = 1`;
sqlTagStore.get`select * from t1 where id = ${id} and active = 1`;
```

The only way of binding parameters in tagged statements is with the `${value}` syntax. Do not add parameter binding placeholders (`?` etc.) to the SQL query string itself.

```js
import { DatabaseSync } from 'node:sqlite';

const db = new DatabaseSync(':memory:');
const sql = db.createSQLTagStore();

db.exec('CREATE TABLE users (id INT, name TEXT)');

// Using the 'run' method to insert data.
// The tagged literal is used to identify the prepared statement.
sql.run`INSERT INTO users VALUES (1, 'Alice')`;
sql.run`INSERT INTO users VALUES (2, 'Bob')`;

// Using the 'get' method to retrieve a single row.
const name = 'Alice';
const user = sql.get`SELECT * FROM users WHERE name = ${name}`;
console.log(user); // { id: 1, name: 'Alice' }

// Using the 'all' method to retrieve all rows.
const allUsers = sql.all`SELECT * FROM users ORDER BY id`;
console.log(allUsers);
// [
//   { id: 1, name: 'Alice' },
//   { id: 2, name: 'Bob' }
// ]
```

**Parameters**

- `maxSize` (number, optional)

**Returns**

- `SQLTagStore` — A new SQL tag store for caching prepared statements.

* **Since:** v24.9.0

<MemberHeading
  id="deserialize"
  depth="3"
  name="deserialize"
  sig="deserialize(
	buffer: Uint8Array,
	options?: DeserializeOptions,
): void"
/>

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L502" sourceLabel="sqlite.d.ts:502" />

_Inherited from&#x20;_`deserialize`

Loads a serialized database into this connection, replacing the current database. The deserialized database is writable. Existing prepared statements are finalized before deserialization is attempted, even if the operation subsequently fails. This method is a wrapper around [`sqlite3_deserialize()`](https://sqlite.org/c3ref/deserialize.html).

```js
import { DatabaseSync } from 'node:sqlite';

const original = new DatabaseSync(':memory:');
original.exec('CREATE TABLE t(key INTEGER PRIMARY KEY, value TEXT)');
original.exec("INSERT INTO t VALUES (1, 'hello')");
const buffer = original.serialize();
original.close();

const clone = new DatabaseSync(':memory:');
clone.deserialize(buffer);
console.log(clone.prepare('SELECT value FROM t').get());
// Prints: { value: 'hello' }
```

**Parameters**

- `buffer` (Uint8Array) — A binary representation of a database, such as the output of `database.serialize()`.
- `options` (DeserializeOptions, optional) — Optional configuration for the deserialization.

**Returns**

- `void`

* **Since:** v26.1.0

<MemberHeading id="enabledefensive" depth="3" name="enableDefensive" sig="enableDefensive(active: boolean): void" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L320" sourceLabel="sqlite.d.ts:320" />

_Inherited from&#x20;_`enableDefensive`

Enables or disables the defensive flag. When the defensive flag is active, language features that allow ordinary SQL to deliberately corrupt the database file are disabled. See [`SQLITE_DBCONFIG_DEFENSIVE`](https://www.sqlite.org/c3ref/c_dbconfig_defensive.html#sqlitedbconfigdefensive) in the SQLite documentation for details.

**Parameters**

- `active` (boolean) — Whether to set the defensive flag.

**Returns**

- `void`

* **Since:** v25.1.0

<MemberHeading id="enableloadextension" depth="3" name="enableLoadExtension" sig="enableLoadExtension(allow: boolean): void" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L312" sourceLabel="sqlite.d.ts:312" />

_Inherited from&#x20;_`enableLoadExtension`

Enables or disables the `loadExtension` SQL function, and the `loadExtension()` method. When `allowExtension` is `false` when constructing, you cannot enable loading extensions for security reasons.

**Parameters**

- `allow` (boolean) — Whether to allow loading extensions.

**Returns**

- `void`

* **Since:** v22.13.0

<MemberHeading id="exec" depth="3" name="exec" sig="exec(sql: string): void" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L337" sourceLabel="sqlite.d.ts:337" />

_Inherited from&#x20;_`exec`

This method allows one or more SQL statements to be executed without returning any results. This method is useful when executing SQL statements read from a file. This method is a wrapper around [`sqlite3_exec()`](https://www.sqlite.org/c3ref/exec.html).

**Parameters**

- `sql` (string) — A SQL string to execute.

**Returns**

- `void`

* **Since:** v22.5.0

<MemberHeading id="function" depth="3" name="function" sig="function" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L349" sourceLabel="sqlite.d.ts:349" />

_Inherited from&#x20;_`function`

This method is used to create SQLite user-defined functions. This method is a wrapper around [`sqlite3_create_function_v2()`](https://www.sqlite.org/c3ref/create_function.html).

- **Since:** v22.13.0

<Signature
  code="function(
	name: string,
	options: FunctionOptions,
	fn: (args: SQLOutputValue[]) => SQLInputValue,
): void"
/>

**Parameters**

- `name` (string) — The name of the SQLite function to create.
- `options` (FunctionOptions) — Optional configuration settings for the function.
- `fn` ((args: SQLOutputValue\[]) => SQLInputValue) — The JavaScript function to call when the SQLite function is invoked. The return value of this function should be a valid SQLite data type: see [Type conversion between JavaScript and SQLite](https://nodejs.org/docs/latest-v26.x/api/sqlite.html#type-conversion-between-javascript-and-sqlite). The result defaults to `NULL` if the return value is `undefined`.

**Returns**

- `void`

<Signature
  code="function(
	name: string,
	fn: (args: SQLOutputValue[]) => SQLInputValue,
): void"
/>

This method is used to create SQLite user-defined functions. This method is a wrapper around [`sqlite3_create_function_v2()`](https://www.sqlite.org/c3ref/create_function.html).

**Parameters**

- `name` (string) — The name of the SQLite function to create.
- `fn` ((args: SQLOutputValue\[]) => SQLInputValue) — The JavaScript function to call when the SQLite function is invoked. The return value of this function should be a valid SQLite data type: see [Type conversion between JavaScript and SQLite](https://nodejs.org/docs/latest-v26.x/api/sqlite.html#type-conversion-between-javascript-and-sqlite). The result defaults to `NULL` if the return value is `undefined`.

**Returns**

- `void`

<MemberHeading id="loadextension" depth="3" name="loadExtension" sig="loadExtension(path: string): void" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L304" sourceLabel="sqlite.d.ts:304" />

_Inherited from&#x20;_`loadExtension`

Loads a shared library into the database connection. This method is a wrapper around [`sqlite3_load_extension()`](https://www.sqlite.org/c3ref/load_extension.html). It is required to enable the `allowExtension` option when constructing the `DatabaseSync` instance.

**Parameters**

- `path` (string) — The path to the shared library to load.

**Returns**

- `void`

* **Since:** v22.13.0

<MemberHeading id="location" depth="3" name="location" sig="location(dbName?: string): string" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L329" sourceLabel="sqlite.d.ts:329" />

_Inherited from&#x20;_`location`

This method is a wrapper around [`sqlite3_db_filename()`](https://sqlite.org/c3ref/db_filename.html)

**Parameters**

- `dbName` (string, optional) — Name of the database. This can be `'main'` (the default primary database) or any other database that has been added with [`ATTACH DATABASE`](https://www.sqlite.org/lang_attach.html) **Default:** `'main'`.

**Returns**

- `string` — The location of the database file. When using an in-memory database, this method returns null.

* **Since:** v24.0.0

<MemberHeading id="open" depth="3" name="open" sig="open(): void" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L454" sourceLabel="sqlite.d.ts:454" />

_Inherited from&#x20;_`open`

Opens the database specified in the `path` argument of the `DatabaseSync`constructor. This method should only be used when the database is not opened via the constructor. An exception is thrown if the database is already open.

**Returns**

- `void`

* **Since:** v22.5.0

<MemberHeading id="prepare" depth="3" name="prepare" sig="prepare(sql: string, options?: PrepareOptions): StatementSync" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L511" sourceLabel="sqlite.d.ts:511" />

_Inherited from&#x20;_`prepare`

Compiles a SQL statement into a [prepared statement](https://www.sqlite.org/c3ref/stmt.html). This method is a wrapper around [`sqlite3_prepare_v2()`](https://www.sqlite.org/c3ref/prepare.html).

**Parameters**

- `sql` (string) — A SQL string to compile to a prepared statement.
- `options` (PrepareOptions, optional) — Optional configuration for the prepared statement.

**Returns**

- `StatementSync` — The prepared statement.

* **Since:** v22.5.0

<MemberHeading id="prepareforruntime" depth="3" name="prepareForRuntime" sig="prepareForRuntime(): void" />

<MemberMeta sourceHref="/source/backend/users/userdb-ts/#L30" sourceLabel="UserDB.ts:30" />

**Returns**

- `void`

<MemberHeading id="serialize" depth="3" name="serialize" sig="serialize(dbName?: string): NonSharedUint8Array" />

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L475" sourceLabel="sqlite.d.ts:475" />

_Inherited from&#x20;_`serialize`

Serializes the database into a binary representation, returned as a `Uint8Array`. This is useful for saving, cloning, or transferring an in-memory database. This method is a wrapper around [`sqlite3_serialize()`](https://sqlite.org/c3ref/serialize.html).

```js
import { DatabaseSync } from 'node:sqlite';

const db = new DatabaseSync(':memory:');
db.exec('CREATE TABLE t(key INTEGER PRIMARY KEY, value TEXT)');
db.exec("INSERT INTO t VALUES (1, 'hello')");
const buffer = db.serialize();
console.log(buffer.length); // Prints the byte length of the database
```

**Parameters**

- `dbName` (string, optional) — Name of the database to serialize. This can be `'main'` (the default primary database) or any other database that has been added with [`ATTACH DATABASE`](https://www.sqlite.org/lang_attach.html). **Default:** `'main'`.

**Returns**

- `NonSharedUint8Array` — A binary representation of the database.

* **Since:** v26.1.0

<MemberHeading
  id="setauthorizer"
  depth="3"
  name="setAuthorizer"
  sig="setAuthorizer(
	callback: (actionCode: number, arg1: string, arg2: string, dbName: string, triggerOrView: string) => number,
): void"
/>

<MemberMeta sourceHref="/source/node-modules/types/node/sqlite-d-ts/#L402" sourceLabel="sqlite.d.ts:402" />

_Inherited from&#x20;_`setAuthorizer`

Sets an authorizer callback that SQLite will invoke whenever it attempts to access data or modify the database schema through prepared statements. This can be used to implement security policies, audit access, or restrict certain operations. This method is a wrapper around [`sqlite3_set_authorizer()`](https://sqlite.org/c3ref/set_authorizer.html).

When invoked, the callback receives five arguments:

- `actionCode` {number} The type of operation being performed (e.g., `SQLITE_INSERT`, `SQLITE_UPDATE`, `SQLITE_SELECT`).
- `arg1` {string|null} The first argument (context-dependent, often a table name).
- `arg2` {string|null} The second argument (context-dependent, often a column name).
- `dbName` {string|null} The name of the database.
- `triggerOrView` {string|null} The name of the trigger or view causing the access.

The callback must return one of the following constants:

- `SQLITE_OK` - Allow the operation.
- `SQLITE_DENY` - Deny the operation (causes an error).
- `SQLITE_IGNORE` - Ignore the operation (silently skip).

```js
import { DatabaseSync, constants } from 'node:sqlite';
const db = new DatabaseSync(':memory:');

// Set up an authorizer that denies all table creation
db.setAuthorizer((actionCode) => {
  if (actionCode === constants.SQLITE_CREATE_TABLE) {
    return constants.SQLITE_DENY;
  }
  return constants.SQLITE_OK;
});

// This will work
db.prepare('SELECT 1').get();

// This will throw an error due to authorization denial
try {
  db.exec('CREATE TABLE blocked (id INTEGER)');
} catch (err) {
  console.log('Operation blocked:', err.message);
}
```

**Parameters**

- `callback` ((actionCode: number, arg1: string, arg2: string, dbName: string, triggerOrView: string) => number) — The authorizer function to set, or `null` to clear the current authorizer.

**Returns**

- `void`

* **Since:** v24.10.0

<MemberHeading id="setup" depth="3" name="setup" sig="setup(): Promise<void>" />

<MemberMeta badges="async" sourceHref="/source/backend/users/userdb-ts/#L22" sourceLabel="UserDB.ts:22" />

**Returns**

- `Promise<void>`

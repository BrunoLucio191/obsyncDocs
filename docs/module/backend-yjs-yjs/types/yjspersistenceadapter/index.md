---
title: YjsPersistenceAdapter
kind: typedef
longname: module:backend/yjs/yjs.types.YjsPersistenceAdapter
---

# YjsPersistenceAdapter

<Signature
  code="YjsPersistenceAdapter = {
	bindState: (docName: string, ydoc: Y.Doc) => Promise<void>;
	deleteStateUnderPath?: (targetPath: string) => Promise<void>;
	destroyState?: (docName: string, ydoc: Y.Doc) => Promise<void> | void;
	renameStatePath?: (oldPath: string, newPath: string) => Promise<void>;
	writeState: (docName: string, ydoc: Y.Doc) => Promise<void>;
}"
/>

<SourceLink href="/source/backend/yjs/yjs-types-ts/#L3" label="yjs.types.ts:3" />

**Properties**

- `bindState` ((docName: string, ydoc: Y.Doc) => Promise\<void>)
- `deleteStateUnderPath` ((targetPath: string) => Promise\<void>, optional)
- `destroyState` ((docName: string, ydoc: Y.Doc) => Promise\<void> | void, optional)
- `renameStatePath` ((oldPath: string, newPath: string) => Promise\<void>, optional)
- `writeState` ((docName: string, ydoc: Y.Doc) => Promise\<void>)

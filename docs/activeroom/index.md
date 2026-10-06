---
title: ActiveRoom
kind: typedef
longname: ActiveRoom
---

# ActiveRoom

<Signature
  code="ActiveRoom = {
	closing: boolean;
	fileName: string;
	networkDoc: Y.Doc;
	networkEnabled: boolean;
	onAwarenessChange: (change: AwarenessChange) => void;
	onBrowserOnline: () => void;
	onConnectionClose: () => void;
	onNetworkUpdate: ((update: Uint8Array) => void) | null;
	onVisibilityChange: () => void;
	pendingLeaveTimers: Map<string, number>;
	persistence: OfflinePersistenceHandle;
	persistenceReady: boolean;
	provider: WebsocketProvider;
	reconnectDelayMs: Backoff;
	remoteClients: Map<number, RemotePresence>;
	remoteUserClients: Map<string, Set<number>>;
	requestWebSocketTicket: () => Promise<string | null>;
	ticketReconnectTimer: number | null;
	ticketRequestInFlight: boolean;
	ydoc: Y.Doc;
}"
/>

<SourceLink href="/source/plugin/obsync/src/collab/collab-types-ts/#L36" label="collab.types.ts:36" />

**Properties**

- `closing` (boolean)
- `fileName` (string)
- `networkDoc` (Y.Doc)
- `networkEnabled` (boolean)
- `onAwarenessChange` ((change: [AwarenessChange](/awarenesschange)) => void)
- `onBrowserOnline` (() => void)
- `onConnectionClose` (() => void)
- `onNetworkUpdate` (((update: Uint8Array) => void) | null)
- `onVisibilityChange` (() => void)
- `pendingLeaveTimers` (Map\<string, number>)
- `persistence` ([OfflinePersistenceHandle](/offlinepersistencehandle))
- `persistenceReady` (boolean)
- `provider` (WebsocketProvider)
- `reconnectDelayMs` ([Backoff](/backoff))
- `remoteClients` (Map\<number, [RemotePresence](/remotepresence)>)
- `remoteUserClients` (Map\<string, Set\<number>>)
- `requestWebSocketTicket` (() => Promise\<string | null>)
- `ticketReconnectTimer` (number | null)
- `ticketRequestInFlight` (boolean)
- `ydoc` (Y.Doc)

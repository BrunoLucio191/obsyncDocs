---
title: RouteSyncFilesContructor
kind: typedef
longname: RouteSyncFilesContructor
---

# RouteSyncFilesContructor

<Signature
  code="RouteSyncFilesContructor = {
	adminMiddleware: (req: Request, res: Response, next: NextFunction) => void;
	authMiddleware: (req: Request, res: Response, next: NextFunction) => Promise<void>;
	clientIdMiddleware: (req: Request, res: Response, next: NextFunction) => void;
	syncfilesController: SyncFilesController;
}"
/>

<SourceLink href="/source/backend/server/expressserver/routes/route-syncfiles-ts/#L5" label="route.syncFiles.ts:5" />

**Properties**

- `adminMiddleware` ((req: Request, res: Response, next: NextFunction) => void)
- `authMiddleware` ((req: Request, res: Response, next: NextFunction) => Promise\<void>)
- `clientIdMiddleware` ((req: Request, res: Response, next: NextFunction) => void)
- `syncfilesController` ([SyncFilesController](/syncfilescontroller))

---
title: AuthControllerContructor
kind: typedef
longname: AuthControllerContructor
---

# AuthControllerContructor

<Signature
  code="AuthControllerContructor = {
	accountLoginRateLimiter: LoginRateLimiter;
	authService: AuthService;
	dbService: DBServices;
	ipLoginRateLimiter: LoginRateLimiter;
	passwordChangeRateLimiter: LoginRateLimiter;
	queueManager: QueueManager;
	tokenService: TokenService;
}"
/>

<SourceLink href="/source/backend/server/expressserver/controllers/authcontroller-ts/#L15" label="AuthController.ts:15" />

**Properties**

- `accountLoginRateLimiter` ([LoginRateLimiter](/loginratelimiter))
- `authService` ([AuthService](/authservice))
- `dbService` ([DBServices](/dbservices))
- `ipLoginRateLimiter` ([LoginRateLimiter](/loginratelimiter))
- `passwordChangeRateLimiter` ([LoginRateLimiter](/loginratelimiter))
- `queueManager` ([QueueManager](/queuemanager))
- `tokenService` ([TokenService](/tokenservice))

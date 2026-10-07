---
title: AuthControllerContructor
kind: typedef
longname: module:backend/Server/ExpressServer/controllers/AuthController.AuthControllerContructor
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

- `accountLoginRateLimiter` ([LoginRateLimiter](/module/backend-auth-loginratelimiter/loginratelimiter))
- `authService` (AuthService)
- `dbService` ([DBServices](/module/backend-users-dbservices/dbservices))
- `ipLoginRateLimiter` ([LoginRateLimiter](/module/backend-auth-loginratelimiter/loginratelimiter))
- `passwordChangeRateLimiter` ([LoginRateLimiter](/module/backend-auth-loginratelimiter/loginratelimiter))
- `queueManager` (QueueManager)
- `tokenService` ([TokenService](/module/backend-auth-tokenservice/tokenservice))

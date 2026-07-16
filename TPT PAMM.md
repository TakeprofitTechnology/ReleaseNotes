# TPT PAMM

## Version 2026.6.16.737 (16 June, 2026)
* Improved the reliability of MT5 balance operations by introducing an automatic retry queue. Failed operations are now retried using a configurable backoff schedule before being marked as failed, while completed operations are never executed twice. 
* Added operation lifecycle tracking, retry metadata, and administrative API endpoints for monitoring, retrying, cancelling, and manually resolving balance operations.
* Added idempotency protection for MT5 balance operations to prevent duplicate deposits and withdrawals during retries, worker restarts, or temporary failures. Each operation is uniquely identified, protected against concurrent processing with worker locks, and validated before execution to ensure completed operations are never sent to MT5 more than once.
* Added a Risk Score for leaders based on trading performance and risk metrics. The score is displayed throughout the platform and can be used to sort leader rankings by lowest or highest risk.

## Version 2026.6.8.595 (8 June, 2026)
* Added a new Operations administration page for monitoring and managing asynchronous operations. Administrators can view operation statuses, inspect detailed execution history, retry failed operations, cancel pending or failed operations, and manually resolve completed operations. All manual actions require confirmation and are recorded in the audit log.
* Added configurable Investment Stop Loss to automatically protect investments when a predefined loss threshold is reached.


## Version 2026.5.27.597 (27 May, 2026)
* Python backend (server-python/) archived to branch archive/python-backend — no longer part of the main codebase. Master now runs .NET only.
* Settlement "Settling…" badge incorrectly appeared on old Stopped/Cancelled investments when a sibling investment was being settled. Now correctly scoped per stop event.
* Investor's "Invested" label on My Investments page showed running balance (which is 0 after Stop) instead of the original invested principal.
* After stopping an investment with a leader, the "Invest" button was disabled — now correctly re-enabled for re-investment with the same leader.
* "Total Invested" header now sums only lifecycle-active investments (excludes stopped ones).
* My Investments page now sorts newest-first by creation date.
* "Settling… outbox in flight" wording replaced with "Settling… this usually takes a few seconds" (removes internal terminology from user-facing UI).
* request_key column from the balance operation outbox — duplicate prevention is already handled by DB constraints and processing logic.

## Version 0.0.0.4 (26 May, 2026)
* Floating P&L share model — investors' profit/loss floats with the leader's MT5 balance between crystallization events (Stop, Withdraw, Partial Withdraw). No per-deal pushes.
* CrystallizationService — on a crystallization trigger, snapshots positions, force-closes them via MT5 Manager API, calculates pro-rata P&L distribution across all active investors, reopens positions, and commits all changes atomically.
* BalanceOpOutboxWorker — single-shot balance operation delivery to MT5. On failure, the row stays failed until an operator resolves it manually (no automatic retries to prevent double-crediting).
* InvestmentReconciler — moves investments from Pending to Active after MT5 confirms the deal.
* Async-accept API pattern — all mutating PAMM endpoints (/start, /stop, /withdraw, /partial-withdraw) return 202 Accepted with { operationId, status: "pending" } immediately; client polls for settlement status.
* hasPendingSettlement / needsOperatorAttention flags on investor cards — surfaces "Settling…" and "Settlement issue" states in the UI.
* Admin operator recovery surface — POST /api/admin/pamm/outbox/{id}/resolve and POST /api/admin/pamm/investments/{id}/resolve for manually resolving stuck operations.
* Read-only MT5 Leader Dashboard — leaders see their positions, balance, and linked investors; no demo trading UI.
* Demo trading surface — TradingController, position/quote SignalR hubs, Binance price provider, demo order/position endpoints, and all related frontend components removed.
* Investor dashboard pivots to the crystallization flow — shows floating share value, invested principal, and settlement status.

## Version 0.0.0.3 (21 May, 2026)
* Authentication migrated from JWT Bearer tokens to HTTP-only cookies (TakeProfit.PAMM.Auth, SameSite=Lax, 1-day sliding expiration). No more tokens in localStorage or ?access_token= query parameters.
* Credential encryption replaced — custom AES-256-CBC scheme replaced by ASP.NET Core IDataProtector (AES + HMAC), with DPAPI protection at rest on Windows. Existing MT5 credentials must be re-entered after upgrade.
* App settings rebuilt to the Hub WebProtocolSettings pattern — simplified appsettings.json, legacy AllowedHosts/Jwt fields removed.
* JWT from the .NET backend entirely — no JWT keys in source code anywhere.
* GET /api/time endpoint — returns current MT5 server time; used by the client to sync clocks instead of trusting browser local time.
* Typed exception hierarchy — PammException family with global ApiExceptionFilter; all API error responses now return {"message": "..."} consistently (Hub-style), across HTTP and SignalR.
* Configuration page rebuilt — removed connector selector, default symbol, TradeLocker fields, and the symbol settings table. Platform is now MetaTrader 5 only.
* Symbol contract size and margin-per-lot now sourced live from MT5 (5-minute cache) instead of a local symbol_settings database table.
* GET /api/symbol-settings endpoint and symbol_settings database table.
* TradeLockerConnector from both .NET and Python backends.

## Version 0.0.0.3 (19 May, 2026)
* Public landing page — the root / route now redirects directly to /login.
* Authenticated users are redirected from /login to their role-specific dashboard (settings for admin, dashboard for leader, investments for investor).

## Version 0.0.0.2 (20 April, 2026)
* MT5 Manager API as the leader data source — leader accounts are fetched from MT5 rather than managed locally.
* Investor accounts sourced from MT5 — investor login, balance, and group membership resolved via MT5 Manager API.
* Investment start/stop flow with MT5 connection validation — investments require an active MT5 connection on both leader and investor sides.
* MT5 leader group mask filtering with wildcard matching — leaders are identified by configurable group name patterns.
* Inline form validation on the MT5 Connection modal — address, port, credentials validated before submission.
* Delete confirmation dialog for MT5 connections.
* Investor dashboard shows available leaders sourced from MT5, with start/stop investment actions.
* MT5 connection manager bugs — reconnection stability, credential handling, error messages on duplicate connection names.
* Redirect logged-in users from /login to their dashboard (prevents re-authentication loop).


## Version 0.0.0.1 (9 April, 2026)
* Initial .NET (ASP.NET Core) backend with React 19 + TypeScript frontend.
* CI/CD pipeline — GitHub Actions workflows for .NET build + tests, frontend build + type-check, and automated bundle creation (Autobundler).
* Windows Service installer and installation scripts for deployment.
* Three-role system: Administrator, Leader (formerly Trader), Investor — with role-based dashboard routing.
* Basic investment UI — My Investments page, leader cards, deposit flow (demo).
* SPA build paths (wwwroot), npm install compatibility, autobuilder workflow.

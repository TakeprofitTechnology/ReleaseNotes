# TPT PAMM


## Version 2026.8.13.570 (13 August, 2026)
* Investors now always land on the Overview page after signing in, including first-time users with no investments.

## Version 2026.8.6.599 (6 August, 2026)
* Added Leader Profiles with automatically generated performance statistics based on MT5 trading history, including activity before joining PAMM. Profiles include ROI, PnL, AUM, drawdown, volatility, risk score, charts, and other key trading metrics.
* Improved investor exits by proportionally reducing open positions instead of closing and reopening the entire portfolio, minimizing unnecessary spread and slippage for remaining investors.
* Fixed investment P/L calculation to ensure investors only receive profits or losses generated after they join the pool, including movements on positions opened before they joined.
* Improved P/L reporting so Realized and Open Positions P/L are now calculated live and update when the leader closes a position, without waiting for settlement.

## Version 2026.7.29.579 (29 July, 2026)
* Improved live updates for PAMM leader statistics by refreshing the investor count alongside AUM every ~5 seconds after investment changes.
* Added a requirements checklist to the leader list, showing how many requirements each leader currently meets.
* Improved investor and leader management, including complete account lists, faster leader history and risk data, correct account names, and server-specific leader visibility.
* Improved reconciliation and investment processing, preventing false reports and ensuring stopped investments update correctly.
* Improved MT5 integration and stability, including connection re-creation and reduced unnecessary logging.
* Prevented adding duplicate MT5 server connections to PAMM, avoiding duplicate accounts and incorrect equity histories.
* Moved Settings from the top bar to the left sidebar, where it now appears as the last navigation item for all user roles.
* Improved sign-in handling: if the trading server cannot be reached, users now see “Sign-in is temporarily unavailable” instead of an incorrect credentials error.
* Fixed API error responses, recurring resolved accounting issues, and orphaned stop-loss rules that could block new investments.
* Fixed exits from fully depleted investment pools, so investors can stop an investment without repeated errors.
* Corrected displayed and recorded losses so they cannot exceed the investment’s current booked principal.

## Version 2026.7.27.1249 (27 July, 2026)
* Leader avatars are now displayed consistently across the admin console, investor lists, investment portfolio, invest wizard, and leader sidebar.
* Added automatic MT5 connection recovery, restoring dropped connections without manual intervention.
* Improved connection monitoring with regular health and liveness checks and automatic configuration reload after connection settings are changed.
* Added safe MT5 connection deletion, preventing connections from being removed while they have active investments, pending operations, or financial operations in progress.
* Added pagination to the notification bell, allowing users to browse all unread and historical notifications while keeping the Recent tab limited to the latest 20.
* Fixed incorrect profit/loss and stop-loss calculations for legacy investments when broker credit is added after the investment starts.
* Improved handling of unavailable credit data to prevent incorrect calculations and stop-loss triggers.
* Added an admin Rebaseline action to repair stuck leader accounts and unblock investor payouts, with a preview and confirmation before applying changes.
* Improved related reconciliation alerts to show the correct detection time and remain visible until resolved.
* Simplified manual reconciliation runs by removing the note requirement, allowing administrators to start a check immediately with Run now.
* Improved reconciliation error details with clear explanations, expected values, and recommended actions for each issue type, making discrepancies easier to investigate and resolve.
* Improved the experience for disabled investors by hiding all options to start new investments while keeping access to leader information and existing investments.
* Added live leader board updates, refreshing AUM, 30-day PnL, investor counts, and charts every 5 seconds without reloading the page.
* Added the default Takeprofit favicon and improved broker branding so custom favicons display correctly across supported formats.
* Improved Performance Chart calculations using Time-Weighted Return (TWR) to exclude the impact of deposits and withdrawals.
* Updated the large performance charts to anchor the Y-axis at zero for a more consistent view.
* Replaced the horizontal navigation with a persistent left sidebar and a simplified top bar, with role-specific navigation for Investors, Leaders, and Administrators.
* Updated leader card badges to icon-only and expanded the main content area to use the available screen width.
* Fixed navigation so Leaders can no longer access the Investor dashboard and are redirected to their own Dashboard.
* Removed the “All leaders” link from the Leader profile page.
* Added historical performance data for Leader profiles, including trading activity from before the Leader joined PAMM.
* Redesigned Allocation in Investor Analytics as a 100% stacked bar, showing each Leader’s share of active investments.
* Added proportional segments and a detailed legend with each Leader’s current value and allocation percentage.
* Admin → Investors now automatically includes MT5 investor accounts matching the configured group mask, even before their first PAMM sign-in.
* Increased the Investment Wizard width to align it with the Leader profile pages and provide more space for content.
* Improved Leader cards by displaying the full risk score without truncation.
* Replaced badge emoji with clean line icons for a more consistent look across Leader cards, lists, and profiles.

## Version 2026.7.20.999 (20 July, 2026)
* Merged the public Leaders page into the investor My Dashboard with direct profile access and one-click investing.
* Removed the public /leaders endpoint and fixed a critical database update issue that could cause user data loss.
* Removed the Leaders navigation button and deprecated the public /leaders endpoint from the login page.
* Prevented investors from reopening the Investment Wizard for leaders they have already invested in.
* Replaced the Invest button with an Already Invested badge for existing investments.
* Added transactional email notifications with configurable user preferences and branded email templates.
* Removed the manual email endpoint (POST /notifications/email) and simplified email delivery status tracking.
* Removed the duplicate Watchlist button from the PAMM user interface.
* Fixed an issue where the risk amount input in PAMM strategy creation incorrectly displayed a leading "0" while typing.
* Added automatic status refresh across TPT PAMM pages to ensure connection status updates without requiring a manual page refresh.
* Investments and Investment History separated: active and processing investments are now shown on the Investments page, while completed investments are available in Investment History.

## Version 2026.7.16.1111  (16 July, 2026)
* Added a leader verification system with Pending, Verified, and Featured statuses.
* Introduced verification badges across leader listings and profiles, along with administrative verification management.
* Added white-label branding with customizable platform appearance, including logos, colors, login page, and branding profiles.
* Applied branding consistently across the platform, including the dashboard, login page, navigation, and email templates.
* Added a centralized real-time Notification Center for Investors, Leaders, and Operators with persistent notification history, read/unread management, and direct navigation to related pages. Profit information is included in settlement notifications rather than as a separate notification.
* Added a new broker administration portal for TPT PAMM with key platform KPIs.
* Added investor management, including search, filtering, balance and investment monitoring, and enable/disable controls.
* Added leader management with verification status, AUM, investor count, and performance information.
* Added access to active, pending, and closed investments.


## Version 2026.7.8.1155  (8 July, 2026)
* Added out-of-the-box HTTP support for authentication, with optional HTTPS configuration documented.

## Version 2026.7.6.993 (6 July, 2026)
* Added Public Leader Profiles with leader biographies, strategy descriptions, key performance metrics, and historical performance charts to help investors evaluate leaders before investing.
* Added Follow Leaders and Watchlist functionality, allowing investors to follow, favorite, and monitor leaders before investing.
* Added Performance History with historical ROI, equity and drawdown charts, monthly returns, and key performance milestones to help investors evaluate long-term consistency.


## Version 2026.7.3.464 (3 July, 2026)
* Fixed the transaction amount sign in Investor Statements. Investment deposits are now shown as negative amounts (funds leaving the investor account), while investment closures and returned funds are shown as positive amounts (funds credited back to the investor account).

## Version 2026.7.2.481 (2 July, 2026)
* Replaced the existing main-page leader section with the full Leaders Board, while keeping the investor’s balance, active investments, and personal account data visible.

## Version 2026.7.1.865 (1 July, 2026)
* Added a guided Investment Onboarding Wizard that walks investors through leader selection, strategy review, investment setup, risk protection, and confirmation.
* Added an Operations Monitoring Dashboard that provides real-time visibility into MT5 connectivity, financial operations, background workers, queue status, and overall system health.
* Added a Reconciliation Service that automatically compares PAMM data with MT5, validates balances, investments, settlements, and financial operations, detects inconsistencies, and provides reconciliation status and issue reporting.

## Version 2026.6.23.348 (23 June, 2026)
* Added Portfolio Analytics with portfolio value, ROI, realized and unrealized PnL, allocation breakdown, investment details, and performance charts.
* Added Leader Rankings with multiple ranking categories, sorting options, and time-based filters to help investors discover and compare leaders.
* Added Leader Badges to highlight leader trust and performance, with badge display across profiles, leader cards, and rankings, and administrative badge management.
* Added Performance Fee support with configurable fee percentages and High Watermark protection, ensuring fees are charged only on new profits during settlement, profit withdrawals, and investment closure.

## Version 2026.6.16.737 (16 June, 2026)
* Improved the reliability of MT5 balance operations by introducing an automatic retry queue. Failed operations are now retried using a configurable backoff schedule before being marked as failed, while completed operations are never executed twice. 
* Added operation lifecycle tracking, retry metadata, and administrative API endpoints for monitoring, retrying, cancelling, and manually resolving balance operations.
* Added idempotency protection for MT5 balance operations to prevent duplicate deposits and withdrawals during retries, worker restarts, or temporary failures. Each operation is uniquely identified, protected against concurrent processing with worker locks, and validated before execution to ensure completed operations are never sent to MT5 more than once.
* Added a Risk Score for leaders based on trading performance and risk metrics. The score is displayed throughout the platform and can be used to sort leader rankings by lowest or highest risk.
* Added public Leader Statistics, including ROI, AUM, investor count, current equity, and key performance metrics to help investors compare leaders.
* Added Investor Statements with portfolio summaries, transaction history, settlement history, and filtering by date, investment, and transaction type.
* Added an Investor Ledger that records all investment-related financial events, including deposits, withdrawals, settlements, performance fees, stop-loss events, and investment closures.

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

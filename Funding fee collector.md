# Funding fee collector


## Version 2026.6.8.975 (8 June, 2026)
### Features
* Failed operations in Operations History now show a clickable badge: clicking it opens a panel explaining the failure in plain language, with technical details available under a collapsible section. Applies to both new and existing failed operations.
* A failure-reason column has been added to the CSV export.
### Changes
* Failed funding fee operations now write a clear warning to the journal identifying the account, symbol, and the exact reason TradeLocker rejected the charge (e.g. insufficient free balance, or fee amount below the 2-decimal-digit minimum).
## Version 2026.6.3.650 (3 June, 2026)
### Features
* Operations & History now has full page navigation with first, previous, next and last arrows, numbered page links with an ellipsis for large ranges, and a per-page selector (50 / 100 / 200) that opens upward so it is never clipped below the screen. The page count always reflects the current search and filter.
### Changes
* Fixed saving a Brand API base URL that is not a valid web address: the value is now rejected at save time with a clear message, and if new settings fail to build a connection the service keeps the last working connection instead of breaking.
* Fixed symbol mapping save returning HTTP 500 when the same symbol was used for both TradeLocker and MT5: the plugin now automatically upgrades the per-platform uniqueness constraint so the same symbol can coexist across both platforms; true same-platform duplicates are still rejected with a proper error.
* Fixed the manual funding cycle trigger reporting success when the MT5 server was disconnected: cycles that cannot run due to an unavailable MT5 connection are now held for retry and show a clear error, while cycles that ran and found no eligible positions continue to show a success result.

## Version 2026.6.2.619 (3 June, 2026)
### Features
* Added a MetaTrader 5 Manager API connection section to the Settings tab (Host, Port, Manager Login, Manager Password).
* Added a dedicated MT5 Symbols & Markups configuration page, with per-symbol markup rules stored independently from TradeLocker mappings.
* Added MetaTrader 5 connector via Manager API: the plugin now reads logins, groups, open positions, and deal history from MT5, and can post balance and withdrawal operations. The MT5 connection status is shown in the header badge.
### Changes
* Fixed the MT5 connector crashing at startup in production builds due to a native library loading failure in single-file deployments.
* Fixed the connection status badge showing "License invalid" when the Brand API server was unreachable or credentials were empty — the badge now correctly reflects the connection state.

## Version 2026.5.30.949 (1 June, 2026)
### Changes
* Fixed funding fees not being paid after plugin restart across a missed trigger time — the plugin now replays missed cycles from the last operator day on startup (up to 24 cycles for a 1-hour interval, 6 for 4-hour, 3 for 8-hour, 2 for 12-hour).
* Changing **Starting time (TL server)** in Settings now takes effect immediately after clicking Apply — no plugin restart required.
* Fixed Manual Cycle Trigger calendar recording a different UTC time in Operations History than what was entered — entered time is now recorded exactly as typed. Dates older than 7 days are rejected inline before submission.
* Importing a CSV on the **Symbols & Markups** page now shows a preview of pending changes before saving; the operator can review, then explicitly Apply or Cancel before any data is written.
* Fixed markup-kind dropdown being clipped behind table rows on the Symbols & Markups page.
* Fixed **Trigger cycle now** taking up to 3 minutes on busy brands — now completes in under 1 second using in-memory caching of account and position data.
* Fixed **Apply to selected** on Symbols & Markups not updating markup values — both value and kind are now applied correctly to all selected rows.
* Fixed date picker in the Trigger Cycle dialog showing locale-specific labels on non-English Windows — always renders in English now.
* Fixed plugin failing to start when stopped during an in-flight funding cycle — recovery now runs in the background after startup, without blocking the service from starting.
* Improved log output: `IdempotencyKeyFingerprint` removed from Info-level logs, verbose masked HTTP response headers suppressed, license key masked, and user-action lines now include the username (e.g. "Settings updated by user 'admin'").

### Version 2026.5.26.945 (27 May, 2026)
### Features
* Initial version of the application has been released. Now only Tradelocker platform is available for use.

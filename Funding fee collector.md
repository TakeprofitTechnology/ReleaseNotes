# Funding fee collector

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

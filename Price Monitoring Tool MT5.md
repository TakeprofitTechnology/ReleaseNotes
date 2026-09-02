# Price Monitoring Tool MT5

## Version 2026.8.28.694 (28 August, 2026)
### Features
* The tool now monitors whether the MT5 server is available and notifies when the server does not respond or connection problems last too long. Recovery is reported as well.
* Two new settings: TcpCheckIntervalSec (default 60) - how often server availability is checked, and ConnectionAlertAfterSec (default 180) - how long a problem must last before a notification is sent.
### Changes
* Server downtime is no longer reported as a price delay or price difference.
* Symbols deleted from the server are no longer monitored, so false price delay notifications for them are no longer sent.
* A misspelt symbol name in Symbols.csv is now reported clearly instead of a generic error.
* Symbol changes on the server are picked up within seconds instead of up to a minute.
* Fewer repeated errors in the log when symbols are missing or unavailable.
## Version 2026.8.20.784 (20 August, 2026)
* Improved monitoring for closed days, overnight and overlapping trading sessions.
* Symbols with no active sessions no longer generate false price alerts.
* Monitoring now continues reliably when individual symbols have configuration or server errors.

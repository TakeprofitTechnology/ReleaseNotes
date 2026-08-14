# Password override tool MT4

## Version 26.08.12.21 (13 August, 2026)
### Features
* The `ManagerLogin` setting now accepts a comma-separated list of manager accounts (e.g. `1000,1001,2000`), and every manager on the list receives the same notifications. A single value keeps working as before; MetaTrader caps the setting at 127 characters (~15-20 logins), and any entry beyond that is dropped with a log message.
* Clients are now required to set their own password after a manager resets it, not only on newly created accounts. Until they do, trading is disabled with an explanatory message, and it is re-enabled automatically once a valid password is set.

## Version 26.04.09.40 (10 April, 2026)
### Changes
* Fixed the situation when password reset initiated by manager triggered emails to user instead of manager.

## Version 26.03.20.55 (25 March, 2026)
### Changes
* Spam in log files has been fixed.

## Version 26.03.16.62 (19 March, 2026)
### Changes
* Initial version has been released.

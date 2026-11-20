# MT5 Three Seven Gateway 


## Version 2026.11.18.728 (18 November, 2026)
* Fixed stop-out requests being incorrectly rejected during the rejection window. Stop-outs are now executed immediately.
* Stop-out executions no longer affect the rejection window for new positions.
* Fixed position closes being incorrectly rejected during the rejection window on hedging and netting accounts.
* The rejection rule now applies only to requests that open new positions, including netting reversals.
* Closing a position no longer starts or extends the rejection window.
* Upgraded the gateway from .NET 9 to .NET 10.

## Version 2024.12.10.1324 (10 December, 2024)
### Changes
* MT5 Gateway API has been updated to v4731;

# MT5 Leverage Limiter

## Version 26.11.12.71 (12 November, 2026)
* Fixed incorrect journal messages for blocked leverage updates.
* Improved LeverageLimit validation (allowed range: 1–2147483647).
* Invalid configurations no longer prevent the plugin from loading and can be corrected without a server restart.
* Invalid runtime changes are rejected while the previous valid limit remains active.

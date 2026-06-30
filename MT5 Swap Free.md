# MT5 Swap Free

## Version 26.06.04.36 (23 June, 2026)
### Changes
* Invalid or missing configuration now fails fast at startup: the plugin refuses to load, the status badge names the broken setting, and a FATAL line is written to the journal — no more misleading "healthy" status with a broken config.
* A bad configuration pushed at runtime is rejected and the previous valid configuration stays active; a broken config never crashes the MT5 trading server, and recovery requires only pushing a valid configuration.
* Swap-free rules file reloads are now applied all-or-nothing: if the new file fails to parse, the previously loaded rules stay in effect.
## Version 26.03.06.87 (13 March, 2026)
### Changes
* Fixed log message in swap deal creation — now correctly displays 'balance deal' or 'commission deal' depending on the UseCommissionType setting, instead of always showing 'commission deal'.

## Version 25.12.12.56 (12 December, 2025)
### Changes
* The parameter "ProcessNettingByDeal" is added to MT plugin settings.

## Version 25.10.22.76 (27 October, 2025)
### Changes
* Processing of REST API requests have been rebuilt.

## Version 25.05.16.68 (16 May, 2025)
### Changes
* Logging has been improved (some values were changed to basic numbers);

## Version 25.04.11.28 (11 April, 2025)
### Features
* Plugin now can also process netting orders;

## Version 25.03.25.52 (25 March, 2025)
### Changes
* Log files were updated. Now accumulated value previously stored in a position is written;

## Version v25.01.17.27 (17 January, 2025)
### Changes
* Added logging for every swap on the server;
* Added validation for swaps at the group level during: plugin start, settings change, and EOD finish;

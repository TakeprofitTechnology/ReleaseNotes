# Dynamic leverage MT5

## Version 26.07.29.86 (30 July, 2026)
### Changes
* Fixed a stale Total margin in the "Margin recalculation report" log. The report is now written whenever the account total margin changes, not only when the plugin changes a managed symbol's leverage rate — so a hedge or a close on a symbol the plugin does not re-leverage now produces a fresh report line. A recalculation where nothing changed still writes nothing.
* Fixed margin-reducing requests being wrongly rejected with a "not enough money" error under Leverage-mode rules when the account held positions on symbols the plugin does not re-leverage (CFD, CFD-Index, Futures). Such symbols are now included in the account's current margin used by the check.
* Index CFD positions now contribute their tick-based margin to the account total instead of counting as zero.
* A symbol whose margin cannot be calculated now keeps its last known value in the report instead of dropping to zero or suppressing the whole report.
* The plugin binary now identifies itself properly: description, original file name and company name are filled in, which makes it easier to get antivirus false-positive alerts cleared.
* Updated the bundled third-party networking, compression, archive and database libraries, and replaced a 13-year-old cryptography library with the one built into Windows. The replacement produces byte-for-byte identical results, so the trading connection is unaffected.
* The plugin is now built with an additional Windows exploit-protection feature enabled, at a cost of about 1% in file size.
* Crashes on broker servers can now be investigated: debugging information is now produced and kept internally, and is not shipped to customers.
## Version 26.07.16.51 (17 July, 2026)
### Changes
* Fixed an issue where Dynamic Leverage could overwrite a position that was still being filled in parts — rolling its size back and changing its open price and external ID. A new optional setting, UpdatePositionsDelayMs (off by default), makes the plugin wait the configured number of milliseconds before it starts processing a newly opened or closing position, so the fill can finish first.
## Version 26.06.25.62 (30 June, 2026)
### Changes
* Fixed a rare issue where honest clients could be incorrectly rejected with "not enough money" errors once order numbers on a server grew past a certain threshold.
* Closed two additional gaps in the EA-burst abuse protection, including a case where a broken price feed could make the protection work against the account instead of protecting it.
* Fixed an issue where the plugin could overwrite an order while a dealer was actively processing it, which could wipe out flags the dealer had just set.
* Improved plugin resilience: a single transient error no longer disables margin enforcement for the whole server, and the plugin's web interface now stops correctly when the plugin itself stops.
* Configuration validation is now stricter: rules with misspelled or invalid values are now rejected with a clear error message instead of being silently accepted and applied incorrectly. A configuration that previously loaded (only because errors were silently ignored) may now be rejected — please review your configuration if this happens after upgrading.
## Version 26.06.17.71 (22 June, 2026)
### Changes
* Fixed CancelPendingIfNoMargin: pending orders rejected for insufficient margin are now reliably removed. Previously the cancellation request was acknowledged by the trade server but the order was not actually deleted, causing MT5 to retry activation thousands of times.

## Version 26.06.02.63 (2 June, 2026)
### Changes
* Added a comprehensive fake-based test framework to the plugin, enabling deterministic unit and integration testing without a live MT5 server.
* Improved configuration validation and error reporting to prevent invalid configurations from being applied while keeping the last valid configuration active.

## Version 26.05.19.43 (25 May, 2026)
### Changes
* Fixed a bug: if there is no positions and orders related to a rule, margin check on closing was skipped even with RejectOnNegativeFMOnClose=true.

## Version 26.04.24.41 (30 April, 2026)
### Changes
* RejectOnNegativeFM parameter has been added.
* 'Groups' parameter has been added to the base plugin.

## Version 26.4.3.63 (3 April, 2026)
### Changes
* Calculates predicted floating PnL (tempPnL) for market open requests based on current ticks and caches it until order execution/rejection.

## Version 26.03.10.72 (12 March, 2026)
### Changes
* Added reject reasons for CancelPendingIfNoMargin parameter. Reasons are added to comment of the order, for the full list of reasons please refer to the user manual.

## Version 26.02.16.46 (2 February, 2026)
### Features
* The parameter CancelPendingIfNoMargin is added to the plugin.


## Version 26.01.13.47 (13 January, 2026)
### Changes
* The negative equity protection is added (for traders it was possible to perform trades even if the equity is negative).


## Version 25.12.11.65 (12 December, 2025)
### Changes
* Fixed the bug with incorrect MarginMultiplier value affected margin recalculation when equity is out of leverage tiers.

## Version 25.11.14.45 (20 November, 2025)
### Changes
* Rules.tsv changed to .ini for backup compatibility.

## Version 25.10.06.71 (6 October, 2025)
### Changes
* Build on the latest 5320 API version has been released.

## Version 25.10.03.45 (3 October, 2025)
### Changes
* Extended orders info in logs.

## Version 25.09.29.67 (29 September, 2025)
### Changes
* Fixed the calculation of 'marginBeforeRecalc' parameter after reopening a position.
* New reasons have been added to plugin logs. 

## Version 25.09.18.50 (22 September, 2025)
### Changes
* Improved order processing to avoid stucking in 'started' state.

## Version 25.08.26.36 (26 August, 2025)
### Changes
* Journal logs have been rebuilt for better user perception.
* Added log messages for volumes out of tiers.

## Version 25.08.11.41 (18 August, 2025)
### Changes
* Added error message for unsupported parameters.

## Version 25.07.22.1226 (22 July, 2025)
### Changes
* The report is divided by lines in MT5 journal.
* ID of the rule is added to report.

## Version 25.06.23.46 (23 June, 2025)
### Changes
* Fixed the bug with DL changed Dealer value with no reason.

## Version 25.06.20.46 (20 June, 2025)
### Changes
* Reports have been added to log files;
* ReportToJournal parameter has been added.

## Version 25.06.04.53 (4 June, 2025)
### Features
* ForceRecalculation parameter has been added.

## Version 25.05.29.55 (29 May, 2025)
### Changes
* Fixed the bug with incorrect multiplier was applied in case of pending orders activation.

## Version v25.02.25.41 (25 February, 2025)
### Changes
* Fixed the bug with incorrect calculation of predicted margin.

## Version v25.02.19.52 (19 February, 2025)
### Features
* AllowLowMarginTrading parameter has been added, which regulates the lower possible limit for opening a position.

## Version v25.01.28.34 (28 January, 2025)
### Changes
* Fixed logging issue.

## Version v25.01.17.48 (17 January, 2025)
### Changes
* Changed reporting style. Minor bugs fixed.

## Version v25.01.14.84 (14 January, 2025)
### Changes
* Fixed the margin update after positions have been hedged.

## Version v24.11.28.42
### Changes
* Fixed a bug with updating not pending orders.

## Version v24.09.06.52 (6 September, 2024)
### Changes
* Changed UseSecurityVolume parameter behaviour if the securities are not set.

## Version 24.08.27.43 (27 August, 2024)
### Changes
* UpdateExistingPositions bug is fixed.

## Version 2024.7.31.719 (31 July, 2024)
### Changes
* Added new leverage mode: equity (distributed).

## Version 1.60 - 1.62 (8 November, 2023 - 27 December, 2023)
### Changes
* Fixed a bug with non-latin charachters encoding conversion.
* Minor bugs are fixed: the rules were not applied under some conditions.

## Version 1.58 (13 October, 2023)
### Features
* Added parameter "UseSecurityVolume".

## Version 1.56 (14 July, 2023)
### Features
* The margin calculation by equity is added.

## Version 1.55 (5 July, 2023)
### Features
* Added the schedule feature - now it is possible to set rules to apply for the specified time period.

## Version 1.53 (6 March, 2023)
### Changes
* BUG fixed: the rules were not applied under some conditiions.

## Version 1.51 (4 August, 2022)
### Changes
* BUG fixed: the accounts that are not under the plugin were still processed by it.
* Minor GUI bugs are fixed.

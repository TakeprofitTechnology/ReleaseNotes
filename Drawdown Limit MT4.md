# Drawdown Limit MT4

## Version 26.09.28.59 (29 September, 2026)
### Changes
* Spaces around a value pushed from the Administrator are now removed, the same as when the settings file is read at startup.

## Version 26.09.21.31 (25 September, 2026)
### Changes
* If a setting or the rules file is missing or invalid, the plugin now refuses to start. The status badge and a FATAL line in the journal name the wrong setting.
* A bad configuration pushed from the Administrator is now rejected. The plugin keeps running on the previous valid configuration.
* A configuration error never takes the MT4 server down.
* The package now includes an empty rules file, so a fresh install with GUI configuration turned on starts normally.
* A negative log size limit is now rejected. Before, it silently turned off log rotation.
* An invalid FirstLimitsCalculation value is now rejected. Before, the first limits calculation was silently skipped.
* An invalid value in the Enabled column of the rules file is now rejected. An empty value still means disabled.
* Rules file errors now show the file, column, value and line number. The header counts as line 1.
* A rejected rules import now returns an error code instead of a success code.
* The daily recalculation no longer stops for everyone when one account can't be read. Archived and deleted accounts are removed from the plugin.
* Deposits and withdrawals are now counted once, on the correct day.
* After the upgrade, an installation with any of the invalid values above will not start until the value is fixed.

## Version 26.03.30.55 (6 April, 2026)
### Changes
* Daily Withdrawal Adjustment mechanism was added — so that withdrawals (e.g. profit sharing) in F-mode are not counted as drawdown.

## Version 26.03.26.42 (26 March, 2026)
### Changes
* Fixed bug: MT4 OnRollover was using groups from plugin settings instead of those defined in the GUI rules.

## Version 25.11.12.32 (12 November, 2025)
### Features
* Drawdown Comment feature has been added for marking the accounts affected by the plugin.

## Version 25.11.07.42 (7 November, 2025)
### Changes
* Fix of Rules.csv on first plugin launch.

## Version 25.06.27.44 (27 June, 2025)
### Changes
* Added readable falal log message for license exceptions.

## Version 24.07.23.27 (23 July, 2024)
### Features
* It is possible now to configure the plugin via Web GUI configurator.

## Version 1.02 (30 November, 2023)
### Changes
* Merged the code bases od Drawdown Limit MT5 and Drawdown Limit MT4.
* Fixed calculation of the DailyLossLimitPercent parameter: MeasuredDailyLoss is now recalculated every day.

## Version 1.01 (16 November, 2023)
### Changes
* Fixed a bug with closing pending orders in the flat balance profit check mode.

## Version 1.00 (14 November, 2023)
### Changes
* Created the first version of the plugin with the followinf parameters: TotalDrawdownLimitPercent, DailyDrawdownLimitPercent, ProfitCheckMode, HighWatermarkMode, IntegrationWebhook, ProfitLimitPercent, FirstLimitsCalculation, LossLimitPercent, DailyLossLimitPercent.

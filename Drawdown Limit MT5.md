# Drawdown Limit MT5

## Version 26.09.28.59 (29 September, 2026)
### Changes
* Internal update of shared code. No change in plugin behaviour.

## Version 26.09.21.31 (25 September, 2026)
### Changes
* If a setting or the rules file is missing or invalid, the plugin now refuses to start. The status badge and a FATAL line in the journal name the wrong setting.
* A bad configuration pushed from the Administrator is now rejected. The plugin keeps running on the previous valid configuration.
* A configuration error never takes the MT5 server down.
* Fixed: a broken configuration could freeze the Administrator and manager connections until the server was restarted.
* Fixed: the periodic limit check could skip all accounts.
* The plugin now picks up new accounts, group changes and deleted accounts right away.
* Invalid values in the rules file, such as text in number fields or negative numbers, are now rejected.
* An invalid value in the Enabled column of the rules file is now rejected. An empty value still means disabled.
* An invalid log level is now rejected. Before, it was ignored.
* Rules file errors now show the file, column, value and line number. The header counts as line 1.
* A rejected rules import now returns an error code instead of a success code.
* The daily recalculation no longer stops for everyone when one account can't be read. Archived and deleted accounts are removed from the plugin.
* Deposits and withdrawals are now counted once, on the correct day.
* If the plugin database can't be opened, the server no longer hangs. The plugin stays inactive and the status badge explains what to fix.
* After the upgrade, an installation with any of the invalid values above will not start until the value is fixed.

## Version 26.04.06.34 (6 April, 2026)
### Changes
* FirstLimitsCalculation added to plugin's default parameters list.
* Daily Withdrawal Adjustment mechanism was added — so that withdrawals (e.g. profit sharing) in F-mode are not counted as drawdown.
* Added support of DNS addresses.

## Version 26.03.06.46 (10 March, 2026)
### Features
* Daily drawdown base mode parameter has been added.

## Version 25.11.07.43 (7 November, 2025)
### Features
* Drawdown Comment feature has been added for marking the accounts affected by the plugin.
* Fix of Rules.csv on first plugin launch.

## Version 24.08.07.36
### Features
* Additional parameters for prop tradng have been added;

## Version 24.07.23.27 (23 July, 2024)
### Features
* It is possible now to configure the plugin via Web GUI configurator.

## Version 1.16 (29 December, 2023)
### Changes
* Moved the trace logs for equity checking to the debug level. The "DebugLogs" value must be set to "false" so that these logs are not written.
* Made it possible to stop the plugin at the moment of database initialisation during the first start.

## Version 1.15 (18 December, 2023)
### Changes
* Made it possible to use decimal values in settings.
* Reduced the time between equity requests from 5 seconds to 2 seconds.

## Version 1.14 (30 November, 2023)
### Changes
* Merged the code bases od Drawdown Limit MT5 and Drawdown Limit MT4.

## Version 1.12-1.13 (17 November, 2023)
### Changes
* Fixed a bug with sending a wrong loss value in email notifications about TotalLossLimit.
* Fixed a limit calculation for DailyLossLimitPercent parameter. The plugin now calculates percentage based on the initial balance instead of the EOD equity.
* The EOD equity is now stored in the plugin's data base instead of the MT5 user record.

## Version 1.11 (16 October, 2023)
### Changes
* Added limits' percentages to email notifications.

## Version 1.10 (6 October, 2023)
### Changes
* Added EOD equity and initial balance to email notifications.

## Version 1.07-1.09 (29 September, 2023)
### Changes
* Added LossLimitPercent parameter.
* Added DailyLossLimitPercent parameter.
* Fixed the format of numbers in logs.

## Version 1.06 (14 September, 2023)
### Changes
* Limit orders are closed now along with open positions.

## Version 1.05 (1 September, 2023)
### Changes
* FirstLimitsCalculation parameter was added;
* Several bugs have been fixed: limits didn't trigger at the end of the day.

## Version 1.03-1.04 (21 August, 2023)
### Changes
* All plugin parameters have default settings now when the plugin starts.
* A bug was fixed: accounts outside of specified groups have worked with the plugin.
* A fatal error was fixed.


## Version 1.02 (21 August, 2023)
### Changes
* All plugin parameters have default settings now when the plugin starts.
* A bug was fixed: accounts outside of specified groups have worked with the plugin before.


## Version 1.01 (18 August, 2023)
### Changes
* A bug was fixed: the plugin wasn't working with new just created accounts.


## Version 1.00 (17 August, 2023)
### Features
* The first version of the plugin was developed.

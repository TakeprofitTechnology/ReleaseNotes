# Drawdown Limit MT5

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

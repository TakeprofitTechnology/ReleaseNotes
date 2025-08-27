# Dynamic leverage MT5

## Version 25.08.26.36 (26 August, 2025)
### Changes
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

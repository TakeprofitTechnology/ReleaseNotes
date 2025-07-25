# Ashira dealer MT4

## Version 25.07.21.38 (21 July, 2025)
### Changes
* Validation that prevents incorrect symbols in slippage fields is added.

## Version 25.06.27.52 (27 June, 2025)
### Changes
* Added readable falal log message for license exceptions.

## Version 6.11 (27 Oct, 2023)
### Changes
* Added a separate script to provide the order execution statistics based on Ashira execution reports and show the number of extra points earned by Ashira for the broker.

## Version 6.09-6.10 (7 Jun, 2023)
### Changes
* Added “RestServerHost” and “RestServerPort” parameters to settings.ini.
* Bug fixed: Ashira ignored the symbol trading session time when applied time delay. Now the delay is interrupted by the ending of trading session time and Ashira rejects the deal.

## Version 6.08 (3 Feb, 2023)
### Features
* Added REST server for configuring;
* Added handling with REST commands;
### Changes
* Added error pop-up if insert wrong settings in GUI;
* Added header to csv file.

## Version 6.07 (29 Dec, 2022)
### Features
* Added a “FiveRulesOnly” parameter to the license file to limit the number of rules set in Ashira.
### Changes
* Several minor bugs are fixed.

## Version 6.05 (16 May, 2022)
### Features
* Multiple GUIs of Ashira can be opened now by running .exe file twice or more.

## Version 6.02 (29 Nov, 2021)
### Changes
* VC runtime dependencies were removed.

## Version 6.01 (17 Nov, 2021)
### Changes
* Fixed GUI bug, related to Metatrader API crash when receiving email notification. 
* Some minor code ### Changes.

## Version 6.00 (24 Aug, 2021)
### Changes
* The GUI (Ashira Config) is rebuilt: the .NET Framework development libraries were replaced by .NET Core libraries.

## Version 5.73 (19 Aug, 2021)
### Changes
* The number of columns in the default file Rules.csv has been changed for all ## Versions of Ashira Dealer.

## Version 5.72 (20 Jul, 2021)
### Changes
* Ashira GUI working logic is changed: pumping logic is removed from the GUI.

## Version 5.69 (26 Jun, 2021)
### Changes
* Logging the rules with ACTION_DEALER is fixed (the action was marked in the logs as unknown before).

## Version 5.66 (12 Jan, 2021)
### Changes
* GUI logic bug (related to incorrect work of “Save” button) is fixed

## Version 5.60 - 5.65 (17 Nov, 2020 - 23 Dec, 2020)
### Changes
* Fixed bugs related to the work of buttons in the GUI;
* Logs divided between folders: fix, main, feeder.

## Version 5.59 (26 May, 2020)
### Changes
* Advanced logs are added;
* Fixed bug when connecting multiple GUI services.

## Version 5.58 (5 Mar, 2020)
### Changes
* Spread difference bug is fixed

## Version 5.57 (22 Oct, 2019)
### Changes
* Spread Management bugs are fixed

## Version 5.56 (22 Oct, 2019)
### Features
* ChangePrice logic is added

## Version 5.52 - 5.55 (9 Sep, 2019 - 13 Oct, 2019)
### Changes
* Fixed some bugs in plugin code. 

## Version 5.51 (4 Apr, 2019)
### Features
* Action RP (REJECT_PENDINGS) is added.
## Version 5.48 (1 Nov, 2018)
### Changes
* Fixed a critical error in the code when the plugin stopped working.

## Version 5.47 (26 Sep, 2018)
### Changes
* Logging optimization: now some messages are logged as "debug" messages.

## Version 5.46 (21 Sep, 2018)
### Changes
* Inner memory logic optimization.

## Version 5.45 (21 Aug, 2018)
### Changes
* Fixed the wrong logic of the actions P and R. 

## Version 5.44 (2 Aug, 2018)
### Changes
* Bug with blocking quotes when there is no rule in Spend management was fixed.

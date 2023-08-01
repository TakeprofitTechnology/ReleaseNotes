# Takeprofit Web GUI Configurator

## Version 1.38-1.39 (21 July, 2023)
### Changes
* DynamicLeverage MT5 GUI: now it isn't allowed to save the rule if symbols/securities fields are not filled;
* DynamicLeverage MT5 GUI: now it isn't allowed to save the rule if groups/logins fields are not filled;
* DynamicLeverage MT5 GUI: now it isn't allowed to edit the groups if logins is already filled;
* DynamicLeverage MT5 GUI: now it isn't allowed to edit the securities if symbols is already filled;
* DynamicLeverage MT5 GUI: Update Existing positions column was renamed to UpdExistingPos;
* DynamicLeverage MT5 GUI: Account exposure limit column was renamed to Account Vol. Limit;
* DynamicLeverage MT5 GUI: an error message text was changed if leverage tiers is filled incorrect;
* DynamicLeverage MT5 GUI: renamed Rule multiplier mode to Mode;
* DynamicLeverage MT5 GUI: the values of Mode parameter have been changed: now it's Leverage (instead of L) and Multiplier (instead of X);
* DynamicLeverage MT5 GUI: Exposure limit column was renamed to Symbol Vol.Limit;
* DynamicLeverage MT5 GUI: the values of VolumeType parameter have been changed: now it's Lots (instead of L) and Exposure (instead of E);

  
## Version 1.37 (7 July, 2023)
### Changes
* The names of the parameters were aligned to center;
* DynamicLeverage MT5 GUI: Lots value was set as a default for VolumeType parameter;
* Kloshira MT4 GUI: Save button is now highlighted if there is unsaved changes;
* Kloshira MT5 GUI: Save button is now highlighted if there is unsaved changes


## Version 1.34-1.35 (4 July, 2023)
### Features
* Added FlexRebate MT4.

### Changes
* Fixed the names of parameters in appsettings.json;
* Fixed issues in GUI (double-clicking was required to change a value of a parameter);
* DynamicLeverage MT5 GUI: just created rule is enabled by default now.

## Version 1.32-1.33 (6 June, 2023)
### Features
* Added new running status error messages in EasyMAM GUI to status column;
* Parameter “REST Host” was renamed on “REST Host:port”.

### Changes
* Minor displaying bugs fixed.

## Version 1.31 (24 May, 2023)
### Changes
* Minor displaying bugs fixed.

## Version 1.28 - 1.30 (14 May, 2023)
### Features
* Added different statuses to the EasyMAM download page in case of no connection.

### Changes
* Made an automatic refresh of the products "connection details" page;
* Fixed visual errors in the text of some messages;
* Fixed stuck on EasyMAM MT4 download page;
* Fixed bug with displaying connection lost message if the connection was interrupted after the master/slave page was loaded in EasyMAM MT4.

## Version 1.27 (25 April, 2023)
### Changes
* Fixed table display error in EasyMAM MT4 GUI;
* Fixed an error that occurred when trying to set up an account to calculate an account with an ID less than 1000;
* Decreased text size in popup windows;
* Added redirection to the last opened GUI page after service restart.

## Version 1.25-1.26 (19 April, 2023)
### Features
* Currency column was added in EasyMAM MT5 GUI;

### Changes
* Fixed text when calculating incentive in EasyMAM MT4 GUI;
* Made redirection on login page after server restart;
* Added error displaying in case of incorrect actions when calculating the incentive in EasyMAM MT4 GUI.

## Version 1.24 (10 April, 2023)
### Features
* Added SerilogSettings to appsetting.json file;
* Added RestRequestsLogging setting to appsettings.json file;
* Added backward compatibility with old appsetting.json file;
* Added Spread Management configurator;

### Changes
* Changed application favicon;
* Added REST requests logging if RestRequestsLogging true;
* Fixed batch functions in EasyMAM MT5 GUI.

## Version 1.22 (17 March, 2023)
### Features
* Added buttons, incentive calculation in specified days (EasyMAM MT5);

### Changes
* Fixed exception while editing symbols in Kloshira MT4 configurator;
* Added unique color to Max Position Exposure card;
* Added checking the version of EasyMAM to prevent using incentive features with old EasyMAM MT5;

## Version 1.21 (14 March, 2023)
### Changes
* Fixed bug, text overlap while adding new configurator;

## Version 1.20 (17 March, 2023)
### Changes
* Added a message, when there are no configurators and the user doesn't have enough rights to create them;
* Added default values to Max Position Exposure MT4 configurator;

## Version 1.19 (10 March, 2023)
### Features
* Added Max Position Exposure MT4 configurator;
* Added Flex Rebate MT5;

### Changes
* Added HTTPS support;
* Fixed symbols updating in Kloshira MT4 configurator;
* Added normalize conversion during discrepancy calculation, in EasyMAM MT5 configurator;
* Fixed restart fix at Kloshira MT4 configurator;
* Fixed bug, error while adding symbols to Kloshira MT4 configurator;
* Fixed bug, error while edition rules in Kloshira MT4 configurator;
* Fixed bug, error while adding rules Dynamic Leverage Advanced MT4;
* Fixed Dynamic Leverage MT5 rules editing;
* Added default values when adding new rule Dynamic Leverage Advanced MT4;

## Version 1.12 (9 February, 2023)
### Changes
* Fixed minor GUI issues;
* Fixed GUI bugs.

## Version 1.11 (3 February, 2023)
### Features
* Added Ashira support;

### Changes
* Added quotes update in Kloshira MT4 symbols tab;
* Fixed GUI bugs;
* Added restriction of card visibility among users;

## Version 1.10 (26 January, 2023)
### Features
* Added card pictures to bundle;

### Changes
* Fixed bug, reconnecting to deleted product;

## Version 1.09 (23 January, 2023)
### Features
* Initial Version was developed.

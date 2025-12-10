# Web GUI сonfigurator

## Version 2025.12.9.879 (10 December, 2025)
### Changes
* MT4 Ashira: Position lifetime has been renamed to Position lifetime (sec).

## Version 2025.11.24.531 (24 November, 2025)
### Changes
* NOP Limit MT5: fixed columns width.

## Version 2025.11.14.783 (14 November, 2025)
### Changes
* EasyMAM MT5: now it's possible to choose many items on the page using shift button.

## Version 2025.11.10.534 (10 November, 2025)
### Changes
* EasyMAM MT5: added a dropdown to the money managers list when attaching.

## Version 2025.11.5.451 (5 November, 2025)
### Changes
* Checkboxes in all major products were aligned on their click.

## Version 2025.10.29.939 (30 October, 2025)
### Changes
* Dynamic Leverage advanced MT4: Enabled parameter has been added to the Rules.
* NOP Limit MT5: Volume unit parameter has been added.
* Swap Control Center: fixed the possibility to add negative free days.

## Version 2025.10.20.520 (20 October, 2025)
### Changes
* Takeprofit Bridge MT5: table aligned.

## Version 2025.10.15.549 (16 October, 2025)
### Changes
* Name of the product is added to the connection details.

## Version 2025.10.15.412 (15 October, 2025)
### Changes
* Menu offset has been fixed.

## Version 2025.10.8.760 (8 October, 2025)
### Changes
* Fixed a bug with WebGUI went on loop by clicking 'back' button in Google Chrome.

## Version 2025.10.7.430 (7 October, 2025)
### Changes
* Some products names have been added to WebGUI where they previously werent displayed.

## Version 2025.10.3.695 (3 October, 2025)
### Changes
* Removed 'Rules' tab for QuoteWatcher MT4.

## Version 2025.9.29.678 (30 September, 2025)
### Changes
* Fixed hints on hovering.
* Long names on cards are now breaks into several lines.
* Takeprofit Bridge MT5: Action names have been changed.
* The processing of the Enter and Tab keys in tables has been corrected.

## Version 2025.9.22.613 (22 September, 2025)
### Changes
* Takeprofit Bridge MT5: fixed missing rule after Rules.csv import.
* Takeprofit Bridge MT5: added color sample to 'Account color'.
* Hints are removed when hovering mouse over the cell
### Features
* Automatic switch to backup server feature has been implemented for the products which are designed for this (Takeprofit Bridge, Drawdown Limit MT5);

## Version 2025.9.4.221 (8 September, 2025)
### Changes
* Fixed error placeholder position.

## Version 2025.9.1.697 (1 September, 2025)
### Changes
* Takeprofit Bridge MT5: Added 'Country' option to Rules.
 
## Version 2025.8.29.457 (1 September, 2025)
### Changes
* Delete button design has been changed.
* Changing orders of the rules applies as rule changing action.

## Version 2025.8.28.853 (28 August, 2025)
### Changes
* DrawdownLimit: fixed columns size & text.
* Fixed checkbox issue with saving a rule.

## Version 2025.8.27.472 (27 August, 2025)
### Changes
* Fixed pages for Takeprofit Bridge MT4.

## Version 2025.8.26.465 (25 August, 2025)
### Changes
* Removed '_console.start.bat' from the WebGUI folder.
* SwapControlCenter: fixed saving popup.
* Headers for multiple products have been fixed to the screen side when scrolling the page for better accessibility.
* Takeprofit Bridge: Tools buttons have been aligned to the current design.
* 'Delete' buttons have been aligned for the following products: Takeprofit Bridge MT4/MT5, Dynamic Leverage MT5.

## Version 2025.8.22.1010 (22 August, 2025)
### Changes
* MT4 Kloshira has been renamed to MT4 Takeprofit Bridge.
* TPT Bridge has been renamed to MT5 Takeprofit Bridge.
* Minor visual improvements.

## Version 2025.8.18.589 (19 August, 2025)
### Changes
* Removed exceptions from logging;
* Max Position Exposure & Ashira Dealer WebGUIs were aligned with the design.

## 2025.8.11.577 (11 August, 2025)
### Changes
* Fixed value validation in the Delay (bridges and ashira) field to support all floating-point interval formats.
* Changed the logging level (from ERROR to WARNING) for validation when clicking the Save Rules button.

## Version 2025.8.5.625 (5 August, 2025)
### Changes
* For Kloshira MT4 GUI the fields Reason and Type are made as dropdown lists.
* SwapControlCenterMT5: 'Charge swap on excess' added to WebGUI rules.

## Version 2025.8.1.539 (1 August, 2025)
### Changes
* Manager API connection of Swap control center MT4 is removed from WebGUI.

## Version 2025.7.28.1258 (28 July, 2025)
### Changes
* Swap control center MT4 GUI is improved.
* Kloshira MT5 GUI: the long values for reason field representation is improved.
* Many minor GUI improvements for Swap control center MT5.

## Version 2025.7.25.581 (25 July, 2025)
### Changes
* The representation of descrepancies in EasyMAM MT5 GUI is improved (minor GUI bugs are fixed).

## Version 2025.7.24.863 (24 July, 2025)
### Changes
* The titles of tabs in NOP MT5 plugin GUI are changed.
* The logic of saving rules for all products is improved.
* The names of columns inside of imported files (NOP limit MT5 plugin) are improved.

## Version 2025.7.22.1226 (17 July, 2025)
### Changes
* The ID of Dynamic leverage MT5 rule is added to each rule line.
* Added checkboxes to NOP limit MT5 plugin.

## Version 2025.7.21.692 (21 July, 2025)
### Changes
* Manager API connection of Swap control center is removed from WebGIU.
* Validation that prevents incorrect symbols in slippage fields (all bridges and dealers) is added.

## Version 2025.7.18.638 (18 July, 2025)
### Changes
* Code is refactored, seevral minor exceptions are fixed.

## Version 2025.7.17.440 (17 July, 2025)
### Changes
* EasyMAM MT5: Fixed message for SetDetachFee without specified period;
* EasyMAM MT5: Fixed SL request sending 0 instead of null while field is empty. Now to reset sl settings in a comment, you need to send null to a user's status [sl:null], not [sl:0]. Now 0 is a valid value;
## Version 2025.7.7.886 (7 July, 2025)
### Changes
* Commission Manager MT5: added Accumulate commissions parameter.


## Version 2025.7.14.864 (14 July, 2025)
### Changes
* The GUI for Quote watcher MT4 plugin is added to the application.

## Version 2025.7.3.805 (7 July, 2025)
### Changes
* Kloshira MT4/5, TPT Bridge: added validation which prevent from saving rules with empty condition fields;
* TPT Bridge: fixed the bug when symbol quotes did not autoupdate if symbols had dot "." in its name;
* Kloshira MT4/5, TPT Bridge: added validation which prevent from saving several completely identical symbols;

## Version 2025.7.3.471 (3 July, 2025)
### Changes
* SwapControlCenterMT5: added 'Swap allowance type' parameter;

## Version 2025.6.30.898 (30 June, 2025)
### Changes
* TPT Bridge: added 'Account color' parameter.
* TPT Bridge: added support of 'cut' version of the bridge;

## Version 2025.6.17.730 (17 June, 2025)
### Changes
* Kloshira MT4: fixed visual representation of action H in default rules;

## Version 2025.6.16.579 (16 June, 2025)
## Changes
* Flex Rebate MT5: Fixed 'Agent 6' field input value;

## Version 2025.5.19.833 (19 May, 2025)
### Changes
* Bridge MT5: Timeout increase from 1 to 30 minutes;
* Bridge MT5: Improved response handling;
* Bridge MT5: Added loading animation on reports button;

## Version 2025.5.15.1176 (15 May, 2025)
### Changes
* NOP Limit: fixed the bug with tables changed width after new rule;
* NOP Limit: tabs removed and replaced with links;

## Version 2025.5.14.687 (14 May, 2025)
### Changes
* SwapControlCenter MT5: fixed a bug with rules could not be saved in WebGUI;
* SwapControlCenter MT5: added CRYPTO swap type;

## Version 2025.5.5.660 (5 May, 2025)
### Changes
* Fixed a bug with cells stuck with empty values and not letting to save the rule;

## Version 2025.4.24.948 (24 April, 2025)
### Changes
* FlexRebate: fixed a bug with 'Object' appearance in blank fields on rule creation;

## Version 2025.4.21.892 (21 April, 2025)
### Changes
* Kloshira/TPT Bridge: default rule has been added;

## Version v2025.4.17.815 (17 April, 2025)
### Features
* Swap Control Center MT4/MT5: Accumulate charge feature has been added;

## Version 2025.4.18.672 (18 April, 2025)
### Features
* Order execution report is added to Reports (TPT bridge MT5).

## Version 2025.4.17.580 (17 April, 2025)
### Changes
* Minor GUI changes for Reports tab of TPT bridge MT5.

## Version 2025.4.16.611 (16 April, 2025)
### Changes
* TPT Bridge: aligned some content so it looks better;
* Swap Control Center: typo fixed;
* NOP Limit: 'Current volume' tab added;

## Version 2025.4.9.806 (9 April, 2025)
### Features
* "Reports" tab is added to TPT bridge MT5 configurator.
* B-book profit report is added to Reports (TPT bridge MT5).

## Version 2025.3.28.764 (28 March, 2025)
### Changes
* SwapControlCenter MT4/5: header was redesigned;
* TPT Bridge: header was redesigned;

## Version 2025.3.18.675 (18 March, 2025)
### Changes
* Now it is possible to see in the log files, which user changed the configuration of products.

## Version 2025.3.13.679 (13 March, 2025)
### Changes
* SwapControlCenter MT5: Fixed the bug with not all the available groups were visible.

## Version 2025.3.14.673 (14 March, 2025)
### Changes
* For Kloshira MT4: WebGUI header has been redesigned;

## Version 2025.3.13.679 (13 March, 2025)
### Changes
* SwapControlCenter MT4: Sunday, Saturday and Disabled values are removed from 'ThreeDaySwaps';

## Version 2025.3.3.709 (3 March, 2025)
### Changes
* Shared accounts volume feature is added to NOP limit MT5 plugin GUI.

## Version 2025.2.24.697 (24 February, 2025)
### Changes
* For Kloshira MT5 and TPT bridge MT5: Symbols tab renamed to A-book symbols.

## Version 2025.2.20.738 (20 February, 2025)
### Changes
* NOP limit MT5 GUI import/export bug is fixed.

## Version 2025.2.18.692 (18 February, 2025)
### Changes
* Kloshira MT4: FIX Sub Account now applies only numberic values;

## Version 2025.1.23.635 (23 January, 2025)
### Changes
* All products: fixed a bug with manual drag & drop of rules didn't work correctly;

## Version 2025.1.13.588 (21 January, 2025)
### Changes
* Swap Manager MT4 - multiple group selection is now available;

## Version 2024.12.16.1138 (16 December, 2024)
### Changes
* All popups were moved to bottom right corner;

## Version 2024.12.18.972 (18 December, 2024)
### Changes
* SwapControlCenterMT5: A new type of commission has been added, 'Commission operation';

## Verstion 2024.12.11.604 (11 December, 2024)
### Changes
* TPT Bridge MT5/Kloshira MT4/Ashira MT4: Added a numerical order in GUI rows;

## Version 2024.12.10.780 (10 December, 2024)
### Changes
* EasyMAM MT4/MT5: Filters have been redesigned;

## Version 2024.12.2.692 (2 December, 2024)
### Changes
* Swap Manager MT5 - multiple group selection is now available;
* Swap Manager MT5 - fixed a bug with delete button not accessible if rules are not filled out;
* Swap Manager MT5 - added a notification after file import;

## Version 2024.11.26.845 (26 November, 2024)
### Changes
* Swap Manager MT5 - fixed naming for exported file;

## Version 2024.11.6.703 (6 November, 2024)
### Changes
* TPTBridge MT5 - added sorting feature;

## Version 2024.9.25.923 (25 September, 2024)
### Changes
* Detach texts have been adjusted;

## Version 2024.9.13.965 (13 September, 2024)
### Changes
* Minor GUI improvements;

## Version 2024.9.12.662 (12 September, 2024)
### Changes
* Dynamic leverage MT5 configurator - rules file can be uploaded in .tsv format;

## Version 2024.7.31.719 (31 July, 2024)
### Changes
* Dynamic leverage MT5 configurator - rules representation bug is fixed. 

## Version 2024.7.30.415 (30 July, 2024)
### Changes
* Minor GUI fixes, some typos are fixed.
* Kloshira MT4 import/export bug is fixed.

## Version 2024.7.2.657 (2 July, 2024)
### Changes
* Fixed the bug when new lines could not be edited properly if several new empty lines were created at the same time.  

## Version 2024.6.24.985 (3 June, 2024)
### Changes
* Several unhandled exceptions were fixed.
* Several minor GUI changes are made (text size, text overlapping).
### Features
* Now it is possible to change the order of configurators with drag and drop.
* It is possible to mark the cards with colors.

## Version 24.5.29.703 (3 June, 2024)
### Changes
*  Kloshira MT4 minor bugs are fixed.

## Version 1.66 (20 May, 2024)
### Changes
* EasyMAM MT5 minor bugs are fixed.
* EasyMAM MT4 minor bugs are fixed.
* Minor GUI changes.

## Version 1.64 (19 April, 2024)
### Changes
* Minor GUI changes.
* Kloshira MT5 GUI field validations are added.

## Version 1.63 (11 April, 2024)
### Changes
* WebGUI logon page is rebuilt.

## Version 1.61 (2 April, 2024)
### Changes
* Dynamic Leverage MT5 GUI is improved.

## Version 1.60 (28 March, 2024)
### Features
* Automatic fee calculation is added for EasyMAM MT5.

## Version 1.46 (19 October, 2023)
### Changes
* Optimised loading of web libraries.
* Changed the names of columns in the Web GUI of MT4 Kloshira.
* Removed space from a toast message in the "Calculate Incentive" field.

## Version 1.45 (16 November, 2023)
### Changes
* Fixed some UI elements.

## Version 1.44 (19 October, 2023)
### Changes
* Changed the link in the footer from "© TakeProfit Technology" to "Takeprofit Tech".
* Fixed the red-underline visual bug in pop-menus.

## Version 1.43 (2 October, 2023)
### Changes
* Fixed an issue with filtering in tables.
* EasyMAM MT5 GUI: removed the ability to edit a cell.
* EasyMAM MT5 GUI: removed "Filter" icon from the first column.
* Dynamic Leverage Advanced MT4 GUI: now an error message appears while trying to add unsupported values in GUI.
* Dynamic Leverage Advanced MT4 GUI: now fractional numbers are supported when adding Levels in leverage rules.


## Version 1.40-1.41 (9 August, 2023)
### Changes
* Added port availability check when setting up the configurator;
* EasyMAM MT5 GUI: fixed display of visual errors when selecting incentive calculation days using the calendar;
* Ashira MT4 GUI: renamed footnote when navigate the mouse to the "Spreads" tab.

## Version 1.38-1.39 (21 July, 2023)
### Changes
* EasyMAM MT5 GUI: column with a checkbox for selecting accounts was added, bulk operations are applied to all selected accounts;
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
* DynamicLeverage MT5 GUI: the values of VolumeType parameter have been changed: now it's Lots (instead of L) and Exposure (instead of E).

  
## Version 1.37 (7 July, 2023)
### Changes
* The names of the parameters were aligned to center;
* DynamicLeverage MT5 GUI: Lots value was set as a default for VolumeType parameter;
* Kloshira MT4 GUI: Save button is now highlighted if there is unsaved changes;
* Kloshira MT5 GUI: Save button is now highlighted if there is unsaved changes.


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
* Currency column was added in EasyMAM MT5 GUI.

### Changes
* Fixed text when calculating incentive in EasyMAM MT4 GUI;
* Made redirection on login page after server restart;
* Added error displaying in case of incorrect actions when calculating the incentive in EasyMAM MT4 GUI.

## Version 1.24 (10 April, 2023)
### Features
* Added SerilogSettings to appsetting.json file;
* Added RestRequestsLogging setting to appsettings.json file;
* Added backward compatibility with old appsetting.json file;
* Added Spread Management configurator.

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
* Added checking the version of EasyMAM to prevent using incentive features with old EasyMAM MT5.

## Version 1.21 (14 March, 2023)
### Changes
* Fixed bug, text overlap while adding new configurator.

## Version 1.20 (17 March, 2023)
### Changes
* Added a message, when there are no configurators and the user doesn't have enough rights to create them;
* Added default values to Max Position Exposure MT4 configurator.

## Version 1.19 (10 March, 2023)
### Features
* Added Max Position Exposure MT4 configurator;
* Added Flex Rebate MT5.

### Changes
* Added HTTPS support;
* Fixed symbols updating in Kloshira MT4 configurator;
* Added normalize conversion during discrepancy calculation, in EasyMAM MT5 configurator;
* Fixed restart fix at Kloshira MT4 configurator;
* Fixed bug, error while adding symbols to Kloshira MT4 configurator;
* Fixed bug, error while edition rules in Kloshira MT4 configurator;
* Fixed bug, error while adding rules Dynamic Leverage Advanced MT4;
* Fixed Dynamic Leverage MT5 rules editing;
* Added default values when adding new rule Dynamic Leverage Advanced MT4.

## Version 1.12 (9 February, 2023)
### Changes
* Fixed minor GUI issues;
* Fixed GUI bugs.

## Version 1.11 (3 February, 2023)
### Features
* Added Ashira support.

### Changes
* Added quotes update in Kloshira MT4 symbols tab;
* Fixed GUI bugs;
* Added restriction of card visibility among users.

## Version 1.10 (26 January, 2023)
### Features
* Added card pictures to bundle.

### Changes
* Fixed bug, reconnecting to deleted product.

## Version 1.09 (23 January, 2023)
### Features
* Initial Version was developed.

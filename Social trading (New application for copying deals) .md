# TPT Social trading

## Version v2024.9.27.846 (27 September, 2024)
### Features
* Several API methods have been implemented;
### Changes
* Swagger page has been modified for recent API update;

## Version v2024.9.24.786 (24 September, 2024)
### Features
* 'Strategy ID' column has been added to 'My positions' and 'History' pages;

## Version v2024.9.20.730 (20 September, 2024)
### Changes
* Copying logic improved on server restart;
* Iternal logging improvement;
* The possibility for leaders with active strategies to become basic followers have been removed;
* Server name can now be changed without reconnecting;
* Error notification texts have been adjusted;
* Minor bugs fix;

## Version v2024.9.17.611 (17 September, 2024)
### Changes
* Minor bugs were fixed;
* Several values in admin GUI are now updated automatically;
* Maximum value for Scaled and Fixed copying modes were set to 1000;
* Minor visual improvements;

## Version v2024.9.13.908 (13 September, 2024)
### Changes
* Minor visual adjustments for trader GUI;

## Version v2024.9.11.572 (11 September, 2024)
### Changes
* Leader fields are now frozen while creating a new account until 'can be leader' checkbox is not activated;
* Minor performance & visual improvements;

## Version v2024.9.3.995 (3 September, 2024)
### Changes
* Several visual bugs have been fixed;
* Search function bug has been fixed;
* Fixed a bug adding non-existing account;
* Some texts adjustments;
* Copied PnL value has been removed for Leader's dashboard;
* Several logs records were adjusted;
* General performance improvements;

## Version v2024.8.30.265 (30 August, 2024)
### Changes
* Minor GUI improvements have been applied;

## Version v2024.8.28.802 (28 August, 2024)
### Features
* New design has been applied to both admin and trader GUI;
## Changes
* Unnessessary messages has been removed from logs; 

## Version 2024.8.13.760 (13 August, 2024)
### Changes
* Sorting order in the 'History' page has been changed from ascending to descending;
* The bug with the copied positions changed their copying mode with the strategy change has been fixed;
* Partial closing/closing of positions follows the initial copying mode, if it has been changed in the process of work;
* Fixed buttons aligning on Registration step;
* The bug with multiple grids on reload page has been fixed;
## Features
* Added a default sorting for 'History' page by 'Open Time' (from newest to oldest positions);

## Version 2024.8.2.865 (2 August, 2024)
### Features
* Added a table-view for the Leaderboard. Already followed Leaders are currently placed in a separate table;
* 'Copying Mode' column has been added to the trader's GUI;
* 'History' page has been added to the trader's GUI;
### Changes
* Volume units have been added;
* Columns aligned accordingly;
* General optimization of the system has been performed;
* Loading animation has been removed;
* The bug with incorrect timezone has been fixed;

## Version 2024.7.31.552 (31 July, 2024)
### Changes
* The bug with wrong PnL showing in 'Copied PnL' is fixed;

## Version 2024.7.24.560 (24 July, 2024)
### Changes
* The bug with stop loss logic is fixed;
* Added sorting option for 'Leaderboard' page;
* Authorization error message has been amended;
* Copying bugs were fixed;

## Version 2024.7.23.748 (23 July, 2024)
### Features
* 'Profile' section added for Leader's dashboard;
* Leader can now see his opened positions in 'My Positions' tab;
* The leader now can set up his fees in 'Profile' dropdown in the dashboard;
* The user can now register both as follower and leader from the login screen;
* Paging has been added for GUI;
* Additional caching set up;
### Changes
* Favicon logo added to the login screen;
* Some fonts were changed;
* 'My Followers' tab was hidden from the follower's GUI;
* Several GUI bugs are fixed;

## Version 2024.7.12.630 (11 July, 2024)
### Changes
* The bug of copy system starts copying only after restart is fixed;

## Version 2024.7.9.775 (9 July, 2024)
### Features
* "My Followers" page added to the Leader's GUI, showing leaders information about their followers.

## Version 2024.7.9.733 (9 July, 2024)
### Changes
* The bug of uncontrolled log files creation is fixed.
* The bug of incorrect closing of copied positions when the leader closes partially is fixed.
* The bug of connection to removed servers is fixed.

## Version 2024.7.8.417 (8 July, 2024)
### Features
* Added ID of the follower account for the MT5 log in 'opening time difference' part.
* "Copied PnL" amount added for Trader's Web GUI.
### Changes
* "Total Profit" was renamed to "Total PnL".
* The bug of different rounding between MT4 and MT5 accounts is fixed.
* The bug with incorrect partial close volume calculation is fixed.

## Version 2024.6.21.752 (21 June, 2024)
### Changes
* The bug of position double copying is fixed.

## Version 2024.6.11.645 (11 June, 2024)
### Changes
* Minor bug fixes.
* Minor GUI changes.

## Version 2024.6.10.705 (10 June, 2024)
### Features
* Daily fee is added.
* The logic of copying limit orders is rebuilt.

## Version 2024.6.4.616 (6 June, 2024)
### Changes
* MT4 subscription bug is fixed.

## Version 0.38 - 0.41 (17 Apr - 10 May, 2024)
### Features
* Added a support of MT4 version 1055.
* Added Stop loss feature.
### Changes
* MT4 reconnection logic is improved.
* MT5 reconnection logic is improved.
* Some minor GUI changes.

## Version 0.37 (17 Apr, 2024)
### Features
* Fixed allocation mode is added.
* Server connection status is added to administrator tab.
### Changes
* The follower positions PnL now is updated automatically.
* The bug of position duplication is fixed.


## Version 0.36 (12 Apr, 2024)
### Features
* Trade GUI is splitted to two tabs.
* The system creates the db automatically when installing the 1st time.

## Version 0.35 (8 Apr, 2024)
### Features
* "Min deposit to follow" is added.
* The poositions that are opened by follower themselves are not displayed in the system.
### Changes
* Several copying logic bugs are fixed. 

## Version 0.33-0.34 (29 Mar, 2024)
### Changes
* Added receiving next deal data from MT4 server to the copy system: Open date, Open time, Direction, Symbol, Volume, Profit;
* Added copying of deals between MT4 servers;
* Added information about deal's PnL to the logs. 

## Version 0.31-0.32 (18 Mar, 2024)
### Changes
* Added receiving account ID, equity and currency data from the MT4 server to the copy system;
* Fixed error arising in the presence of a duplicate deal 

## Version 0.30 (7 Mar, 2024)
### Changes
* Added a registration button to the login page.

## Version 0.29 (29 Feb, 2024)
### Changes
* Fixed bug when account that was created in MT5 while CopySystem was running can be added to CopySystem;
*  "Daily fee" was renamed on "Following fee";
*  "Following fee" logic was added.

## Version 0.28 (19 Feb, 2024)
### Changes
* Remove password column from "Servers" tab;
* Added buttons "cancel" and "delete and close" instead of "ok" button in removing strategy window.

## Version 0.26-0.27 (05 Feb, 2024)
### Changes
* "Subscribtion fee" and "Daily fee" were added in web GUI;
* Refresh table button in web GUI was deleted;
* Added additional check for the existence of an MT5 account when adding an account to the Copysystem;
* Made visual inprovements in GUI.


## Version 0.25 (29 Jan, 2024)
### Changes
* Added display and calculation of ROI statistics;
* Fixed a bug where it was impossible to log into GUI if there was no connection to the server;
* Fixed a bug where a deal could be copied twice.

## Version 0.25 (29 Jan, 2024)
### Changes
* Added display and calculation of ROI statistics;
* Fixed a bug where it was impossible to log into GUI if there was no connection to the server;
* Fixed a bug where a deal could be copied twice.


## Version 0.23-0.24 (22 Jan, 2024)
### Changes
* Processing of netting accounts (groups) by the CopySystem is blocked;
* Made display of open positions in the equity chart;
* Fixed a bug where equity was not displayed correctly in the equity chart;
* Fixed a balance discrepancy error in the Copysystem GUI.

## Version 0.22 (10 Jan, 2024)
### Changes
* Fixed a bug when some deals were not copied between MT5 servers;
* Fixed an error in displaying deals data in the Copysystem GUI.

## Version 0.21 (18 Dec, 2023)
### Changes
* Added a chart displaying the equity of leaders;
* Fixed the behavior where CopySystem constantly wrote an error in the log file when a follower did not have enough money.

## Version 0.20 (11 Dec, 2023)
### Changes
* Added copying of deals between MT5 servers.

## Version 0.19 (6 Dec, 2023)
### Changes
* Added receiving next deal data from MT5 server to the copy system: Open date, Open time, Direction, Symbol, Volume, Profit.

## Version 0.16-0.18 (23 Oct - 27 Nov, 2023)
### Changes
* Increased speed of copying deals in the debug connector (less than 1 ms);
* Fixed a bug of copying deals from more than one leader;
* Added connector connection to MT5 server;
* Added receiving account ID, equity and currency data from the MT5 server to the copy system.

## Version 0.14-0.15 (19 Oct, 2023)
### Changes
* Trader's web GUI has been added;
* Current opene positons has been added in trader's web GUI;
* Table with avaliable leaders has been added in  trader's web GUI;
* Balance, equity, total profit and currency statistic has been added in trader's GUI;
* Balance, equity, total profit and currency statistic has been added in "accounts" tab in admin web GUI;
* The number of trader's accounts that can be subscribed to client in GUI has been reduced to 1;

## Version 0.11-0.13 (05 Oct, 2023)
### Changes
* Added copy logic to the debug connector;
* Added automatic closing of deals when deleting the used strategy on follower accounts;
* Added ability to edit strategy tab;
* 'Invert copying' options was remvoed from strategy tab;
* The number of generated accounts in the debug connector has been reduced to 10;
* Added automatic generation of a folder with text files for each generated account in the debug connector;
* "Fixed" and "Equity" strategies were removed;
* "Profit fee" parameter was removed;
* The time for copying deals in the debug connector has been reduced

## Version 0.08-0.10 (28 Sep, 2023)
### Changes
* Added account generation to the debug connector;
* Added balance and equity generation for debug connector accounts;

## Version 0.07 (21 Sep, 2023)
### Changes
* Removed restictions for clients login and password in GUI;
* Fixed wrong text in the popup window;
* Corrected the company name in the footer on the GUI page;
* Fixed incorrect port display when setting it on the server tab;
* Added support for debug connector.
  

## Version 0.05-0.06 (12 Sep, 2023)
### Changes
* Added the "Strategies" tab to the Administrator GUI;
* Fixed the port setting on the new server creation;
* Created connector interface project.

## Version 0.01-0.04 (Aug 31, 2023)
### Changes
* Created the Administrator GUI;
* Created the followings tabs in the GUI: Accounts, Clients, Servers;
* Added autorization page in GUI;
* Added editing and deleting client accounts;
* Added page for changing account password in GUI.

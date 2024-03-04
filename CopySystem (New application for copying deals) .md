# CopySystem (New application for copying deals)


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

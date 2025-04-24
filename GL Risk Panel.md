# GL Risk Panel

## Version 2025.4.24.767 (24 April, 2025)
### Changes
* Fixed the bug with GL making no attempts to reconnection;

## Version v2025.3.6.592 (6 March, 2025)
### Changes:
* Symbol doubling bug has been fixed;

## Version v2024.12.9.859 (9 December, 2024)
### Changes
* Added the option to ignore certain holidays;

## Version v2024.9.12.902 (12 September, 2024)
### Changes
* Minor bugs have been fixed;
* Issue with connecting to the TPT Bridge has been resolved;

## Version v2024.7.11.857 (11 July, 2024)
### Changes
* Fixed a bug with the error on sending correction trades from Risk Panel.

## Version 1.27 (15 December, 2023)
### Changes
* Optimized the data request logic. Now requests to LPs and MT servers are sent simultaneously in multithreaded mode, instead of sequentially by a single thread.

## Version 1.26 (6 December, 2023)
### Changes
* Fixed a bug with the row height in Maker Dashboard.
* Fixed a bug with a page glitch on the color theme change.
* Changed the notifications' logic in Position Checker. Now, before sending a correction limit notification, we first check if there are any servers that are unavailable and if the volumes on the TotalLPs are equal to 0 or if the volumes on clients are equal to 0. If both conditions are met, the notification is triggered.

## Version 1.25 (22 November, 2023)
### Changes
* Optimized code for the Maker Dashboard.
* Updated syncfusion styles loading for each page.
* Corrected non-consistent behavior of the correction limit values.
* Fixed a bug with unsent messages when connecting to Fortex is unsuccessful.

## Version 1.24 (9 November, 2023)
### Changes
* Fixed the incorrect background color marking of correction values.
* Removed the inner table horizontal scroll bar from SyncServer page.
* Changed the background color of Correction USD column in Position Checker.

## Version 1.23 (23 October, 2023)
### Changes
* Position Checker: a background color of Correction USD column was changed;
* ServerSync: possible issues in code in securities comparison has been fixed.

## Version 1.22 (17 October, 2023)
### Changes
* Exception error has been fixed;
* Added spaces in numbers (separate thousands);
* Position Checker: rows with discrepancies are duplicated on the top of the table now;
* Position Checker: an error in positions calculation has been fixed.

## Version 1.21 (5 October, 2023)
### Changes
* A small bug was fixed: the tool sent additional (not needed) notification when discrepancy has been already fixed.


## Version 1.20 (30 September, 2023)
### Changes
* Internal change: for calculation of positions volume on a coverage account now we use the deals from the trading history;
* Horizontal scroling has been removed;


## Version 1.18-19 (25 September, 2023)
### Changes
* Removed extra space around the table in all tables;
* Maker Dashboard: string with data becomes gray in case if tool can't get data from server;
* Maker Dashboard: if data is not loaded, at last update column shows status "Loading"
* Fixed the width of the progress download bar in "position checker" and "server sync" tabs;
* The data in the Position Checker and Maker Dashboard tables has been aligned;


## Version 1.16-1.17 (18 September, 2023)
### Changes
* Maker Dashboard: added additional data validation;
* Added notification when server is not available;
* Position Checker: now string has a background colour when user moves the mouse cursor over this string;
* Position Checker: now columns are visible even when scrolling the table up or down;
* Maker Dashboard: CSS style was changed to font-variant-numeric: tabular-nums;
* Position Checker: when correction limit was reached, data from "Correction", "Correction USD", "Correction Limit" columns becomes red;
* Position Checker: a bug was fixed, now correction limit can be edited while the data is loading/updating;
* Server sync: it's possible to copy the data from the table by double clicking;
* When correction limit is reached, notification is sent to Telegram chat but with correction in USD value additionally included.
  
### Features:
* Grafana button was added to GUI;


## Version 1.15 (11 September, 2023)
### Changes
* Position Checker: now server names are above WL names in the table;
* Position Checker: a visual bug was fixed, loading bar wasn't shown on the bright theme before;
* Compatibility issues have been resolved.


## Version 1.13-1.14 (1 September, 2023)
### Changes
* Maker Dashboard: all numbers are aligned by the right side now, spaces between numbers removed;
* Position Checker: cell borders have been removed;
* Position Checker: all cells are black now;
* Sidebar was moved to the header of the page;
* Server names have been changed.


## Version 1.12 (24 August, 2023)
### Changes
* Position Checker: on mouse hoover to Correction USD cell a popup with rates appears now (it wasn't before);
* Maker Dashboard: calculation of margin level was fixed for Bitfinex.


## Version 1.11 (22 August, 2023)
### Changes
* Position Checker: table was transposed (strings became columns and vice versa);
* Maker Dashboard: JAFX Live string - margin level value shows empty now. Also calculating of each column (balance/equity/margin etc) of JAFX Live string is shown in logs of the tool now.
  

## Version 1.10 (15 August, 2023)
### Features
* Maker Dashboard: a new string was added - JAFX Live. It represents the summed balance/equity/margin etc. of all accounts under GL-*groups on MT4 Server (JAFX Live).


## Version 1.09 (8 August, 2023)
### Changes
* Position checker: WL string and it's coverage account string have been united. 2 values are showing now only if discrepancy happened.
* Position checker: all numbers became right-aligned and font-variant-numeric: tabular-nums is used for numbers from now on.


## Version 1.08 (2 August, 2023)
### Changes
* Maker Dashboard: if ML Notification isn't set, value in the cell remains empty (? was shown before);
* A visual bug was fixed in SymbolSyncTool;


## Version 1.07 (27 July, 2023)
### Changes
* appsettings.json file was reworked to make it comfortable adding more new functions to Risk Panel.

  


# GL Risk Panel

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

  


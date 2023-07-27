# CopyTrader

## Version 2.30 (2 June, 2023)
### Features
* The first version of CopyTrader Website integration Widget was developed.

## Version 2.28 (21 April, 2023)
### Changes
* CopyTrader services (MT4Worker,SignalCore,SignalWebGUI) consume less GPU and RAM now.
* CopyTrader was updated to the latest Manager API.

## Version 2.27 (3 March, 2023)
### Changes
* Strategy bug was fixed. Now if a strategy (subscription) has the error status, it can be deleted. Earlier it wasn’t possible to delete such a strategy.

## Version 2.24 (31 January, 2023)
### Changes
* Sending additional information to the license server.
* Remove duplicates of files from the bundle.
  
## Version 2.22 (13 December, 2022)

### Features
* Regular fees payment logic changed.
* Added ability to connect together MT4 and MT5 workers.
* Added multiserver support to Signal Core.
* Added server name displaying at gui.
* Added server name to account.

### Changes
* Removed spam of warning messages, MT5Worker.
* Unpaired action buttons at my followers tab.
* Changed name of Reverse Copying.
* Changed profit chart appearance.
* Fixed delete button at followers tab.
* Changed Signal Core config.

## Version 2.20 (9 November, 2022)

### Features
* Filter of masters was changed: now the masters can be filtered by their MetaTrader account name or by their copy trader username and MetaTrader login.
* Force PF button was added to the Administrator panel. It is possible to get fee payments from all followers of the particular master by pressing this button.

### Changes
* Configuration files have been fixed. It was hard to edit them before.
* 2 digits after comma are showing now for balance and equity values in the Graphic Interface.
* ROI calculation was fixed.
* Fee % value of the master is now showing as a whole number. It was shown with 2 digits after the comma before.
* The values of the master statistics were showing incorrectly. It was fixed.
* The scrolling bug in the Graphic Interface was fixed.
* In the Follower tab (Administrator panel) and in the Masters tab (Administrator panel) the action buttons (delete, subscribe, edit) have been moved from the end of the table to the beginning.
* Largest Trade Volume parameter was fixed in the Graphic Interface.
* The names of the columns for parameters have been shortened.

## Version 2.17 (11 October, 2022)

### Features
* Equity of the master column was added to the “All strategies” tab. 

### Changes
* Master accounts weren't showing in the Graphic Interface. It was fixed.
* -0.00 values were shown for some parameters in the Graphic Interface. It was fixed.
* “All strategies" tab and "Master accounts" tab in the Administrator panel have been united to one tab - “Master accounts”.
* MT4 Worker didn’t start. It was fixed.

## Version 2.16 (27 September, 2022)

### Features
* Followers can subscribe to the Master from the Followers tab now.

### Changes
* Tab names in GUI have been shortened.
* Profit chart was changed.
* Some of the master parameters have been moved from the masters tab to the master personal card.
* ROI and Master Balance columns have been removed from the follower tab.

## Version 2.15 (30 August, 2022)

### Changes
* After restarting the machine where copy trader is installed, the Core component didn’t start. It was fixed.

## Version 2.14 (25 August, 2022)

### Features
* Copy trader started supporting Cyrillic in the Graphic Interface.
* The name of the user who logs in is shown now in the Graphic Interface.
* In Equity copying mode the currency of the follower account is converting into the currency of the master now. It was done for precise volume copying.

## Version 2.12 (21 July, 2022)

### Changes
* If the master had a credit on the account, trades didn’t copy to the follower. It was fixed.

## Version 2.11 (14 June 2022)

### Changes
* Error in the Core component was fixed.

## Version 2.8 (8 February, 2022)

### Features
* Added the ability to create accounts for a user by clicking the "Add Account" button.
* Added appearance of accounts in Master Accounts and Follower Accounts.

### Changes
* Fixed a bug with the addition of open positions.
* Optimized the copying process.
* Added additional check of snapshots by date.

## Version 2.7 (2 February, 2022)

### Features
* “Add User” button was added to users tab.
* Added possibility to set a temporary password for users.

### Changes
* Removed unused settings from appsettings.json in GUI and Core.

## Version 2.6 (24 January, 2022)

### Changes
* Added fix positions after balance operation “Performance Fee” at Mt5Worker.

## Version 2.5 (18 January, 2022)

### Features
* Added "Add account" button to Follower Accounts table.
* Added “Delete” button to Follower Accounts table.
* The "Edit" and "Unsubscribe" buttons in Follower Accounts are blocked now if there is no subscription.

### Changes
* Fixed "Invalid JSON string" error when creating a subscription in Manager GUI.
* Fixed bug of closing with zero profit in “TradeRequest = false” mode in CopyTrader MT5.
* Fixed cache error.
* White screen bug fixed in Manager GUI.

## Version 2.4 (14 January, 2022)

### Changes
* Added check for open positions.
* Fixed an issue with backward compatibility of settings.
* Improved trade and query logs.
* Fixed frontend bug when creating a subscription through Manager GUI.

## Version 2.2 (29 December, 2021)

### Features
* Added Users page for users with the Admin role.
* Added a Follower accounts page for users with the Admin role.
* Signal in the GUI is renamed to Follower.
* Added Delete button to Master Accounts table.
* Filters added to the Master Accounts table.
* Added Edit buttons to the Master Accounts table.
* Added "Add account" buttons to the Master Accounts table.
* Added Master accounts page for users with the Admin role.

## Version 2.1 (20 December, 2021)

### Features
* Added user authorization with the Admin role.
* Added user authorization by username and password.

### Changes
* A user with the Admin role was added to the database.
* Added Passwords and Salt column to DB Users table.

## Version 2.0 (16 December, 2021)

### Changes
* Product is divided into two parts: CopyTrader and Multicopy System.

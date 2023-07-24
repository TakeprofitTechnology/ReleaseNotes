# EasyMAM MT5

## Version 6.05-6.06 (9 June, 2023)

### Changes
* Code refactoring done;
* Made optimization of reading logs.

## Version 6.03-6.04 (10 May, 2023)

### Changes
* Fixed behavior and added error logs in case if master or slave account was deleted;
* Added clearing the cache from the information about the rest connection, for the correct GUI work.

## Version 6.02 (19 Apr, 2023)

### Changes
* “VolumeClosed” field for slave account now filled with same value as in “VolumeClosed” as on master account;
* Added error in log in case if “VolumeClosed” field on slave account not equal value in “VolumeClosed” field on master account;
* Added info in log about “date range” in case of “date range” incentive calculation;
* Incentive payment for non-existent account was blocked;
* Fixed log error in case of incentive calculation;
* “DelayBetweenStepsInMs” parameter was added;
* Blocked the ability to attach slave account to the master account with a different currency;
* Blocked the ability to set account for incentive calculation with currency differs from slave/masters accounts currency.

## Version 6.00 (06 Apr, 2023)

### Changes
* The “UsedCurrencyProfitStep” parameter was removed from settings. Now EasyMAM always round up profit digits to the number of symbols entered in the "currency" group setting in MT5 admin;
* “UsedSymbolVolumeStep” parameter was added;
* The application has been reassembled;
* Setting support in “XML” was removed;
* Detach error in case when “UsedCurrencyProfitStep” - true, was fixed;
* Distribution error in case when “UsedCurrencyProfitStep” - true, was fixed;
* “Incentive” tab was added in web GUI;
* “PnL” column was added in web GUI in “Slave” tab;
* Manual input of date range for calculation incentive was blocked.

## Version 5.84-5.86 (15 Mar, 2023)

### Changes

* Added function for calculation incentive in specified interval of days;
* Removed dots from logs that end with numbers.

## Version 5.82-5.83 (15 Mar, 2023)

### Changes

* Slave accounts detach with the "true" value of the “IgnoreOpenTrades” parameter has been fixed;
* Fixed a bug with the allocation of deals between slaves accounts due to a duplicate deal.

## Version 5.81 (10 Mar, 2023)

### Changes

* “UseCurrencyProfitStep” parameter was added. 

## Version 5.80 (02 Mar, 2023)

### Changes

* Fixed incorrect balance rounding error after incentive calculation.

## Version 5.79 (28 Feb, 2023)

### Changes

* Config file replaced with appsettings json file.

## Version 5.77-5.78 (22 Feb, 2023)

### Changes

* Log about “UserNotFound” error has been changed;
* Removed console.bat file;
* Inner logic optimization (code refactoring).

## Version 5.76 (14 Feb, 2023)

### Changes

* Replaced AsyncProducerConsumerQueue to Channel;
* Added Polly using in repeated actions;
* Migrated from XML to JSON setting file.

## Version 5.75 (16 Dec, 2022)

### Changes

* Deleted Manager API error spam.

## Version 5.74 (13 Dec, 2022)

### Changes

* API check error excluded from FATAL logs level.

## Version 5.72 (18 Nov, 2022)

### Changes

* Made visual changes to navigate between "Masters" and "Slave" pages in the GUI.

## Version 5.71 (10 Nov, 2022)

### Changes

* Updated authorization page in the GUI;  
* Added “AllowIncentivePayment” parameter in web GUI;
* Added confirmation for detach in GUI.

## Version 5.70 (8 Nov, 2022)

### Changes

* Added check of master positions volume and slave’s deals on hot detach;  
* Added check of deals deleting on masters and slaves accounts.

## Version 5.69 (16 Oct, 2022)

### Changes

* Made a new visualization for the GUI, adapted to work with a large number of accounts;
* Added manager rights check.

## Version 5.68 (29 Sep, 2022)

### Changes

* Added “IncentivePaymentAfterDetach” to block incentive payment after detach;  
* Added the check of group owner of slaves and masters.

## Version 5.67 (13 Sep, 2022)

### Changes

* Application was completely reassembled, added to the dll files taken out of the “Temp” Windows folder.

## Version 5.66 (09 Sep, 2022)

### Changes

* Fixed bug of discrepancies in position volumes that occurred when redistributing a position during hot deletion;
* Fixed a bug that occurred when there was a discrepancy between the server time and the application time;
* Information about config file added in GUI menu;
* Added balance discrepancy highlighting of “master” and “slaves” accounts in web GUI.

## Version 5.61-5-65 (26 Aug, 2022)

### Changes

* Bug fix: The discrepancy between the balance of slaves and the master when deleting a duplicate deal of the slave has been fixed.
* Bug fix: Skip master’s position split when hot detach slaves from master fixed.
* Bug fix: bug “Can't dequeue dummy position” related to distribution of orders by dummy account fixed.

## Version 5.55-5-60 (16 Aug, 2022)

### Changes

* Added Web GUI for application function execution.
* RestHost and RestPort parameter added to application config file for connecting to Web GUI.

## Version 5.54 (27 Jun, 2022)

### Changes

* Bug fixed: deal distribution error after slave hot detach in IOT = true.

## Version 5.53 (20 Jun, 2022)

### Changes

* Changed ID numbering of slaves deals.
* Optimized the speed of processing slaves deals.

## Version 5.52 (17 Jun, 2022)

### Changes

* Bug fixed: The exception error was caused by incorrect order compression.
* Bug fixed: After partially closing master’s position and hot detach slave with most part of volume, an error occurred related to incorrect distribution of volumes.

## Version 5.51 (10 Jun, 2022)

### Changes

* Bug was fixed: After hot detach swaps were not properly distributed. Now swaps are distributed proportionally to the closed volume.

## Version 5.50 (31 May, 2022)

### Changes

* The application has been reassembled.

## Version 5.46 (28 Apr, 2022)

### Changes

* Bug was fixed: the deal on the Master with a hot detach in IOT=true was split many times and completely closed. Now the split and closing of the deal is proceeding correctly.

## Version 5.44 (27 Apr, 2022)

### Changes

* Log about closing position after split was added.

## Version 5.41 (4 Apr, 2022)

### Changes

* Bug was fixed: Ignore open trades (true) logic of working was corrected. With IOT=true, detach could not be made.

## Version 5.40 (29 Mar, 2022)

### Changes

* Bug was fixed: an error occurred when attaсhing the slave account to the master account.

## Version 5.35 (9 Feb, 2022)

### Changes

* Additional check is added: now EasyMAM checks if no duplicated deals were created by EasyMAM itself.

## Version 5.34 (27 Jan, 2022)

### Changes

* Bug fixed: EasyMAM calculated the volumes wrongly during the detach by the mode "detach without partial closing position on master".

## Version 5.33 (21 Jan, 2022)

### Changes

* Bug was fixed: in some cases EasyMAM had created the duplicated deals for slave accounts’ positions. The logic of deal creation was improved.

## Version 5.32 (29 Dec, 2021)

### Changes

* Inner logic optimization (code refactoring).

## Version 5.31 (25 Dec, 2021)

### Changes

* Fixed a bug that occurs in case of an attempt to detach a slave whose balance is 0 and part of the profit is not paid to the incentive account.

## Version 5.30 (17 Dec, 2021)

### Changes

* The GUI displays errors in the status field. in case of their occurrence.
* Now the slave account does not get the negative balance by the incentive payment if the detach happened. 
* In the earlier versions, slave account got the negative balance if the incetive amount was higher than the balance of slave account.

## Version 5.28 (6 Dec, 2021)

### Changes

* Attach slave with zero balance is now disabled.
* Stop loss is triggered if equity is lower or equal than set value (it was only lower before).
* Detach mode is added:  now it is possible to detach slave account from master and don’t close master’s positions partially.
* Detach mode is added: now it is possible to detach slave account and round the volume of their trades down (earlier EasyMAM rounds it up all the time).
* Inner logic optimization (code refactoring).

## Version 5.27 (1 Dec, 2021)

### Changes

* Fixed the lack of changing the direction of the position on the slave account in case of a change the direction of the deal on the master.

## Version 5.26 (23 Nov, 2021)

### Changes

* Rare hot detach bug was fixed (there was a situation when the position was left on the master account after a rare sequence of actions was made).
* The IgnoreOpenTrades bug was fixed (the profit of closing deals was rounded to integer which was not correct).
* Rare incentive bug was fixed (there was a case when slave account paid incentive but incentive account did not get the payment).


## Version 5.24 (23 Nov, 2021)

### Changes

* DummyPool setting was removed - now EasyMAM uses the pool of 500 dummy deals.
* The rounding logic was improved - now EasyMAM rounds the profits according to MT5 logic.
* Hot detach logic was improved.

## Version 5.21 (22 Nov, 2021)

### Changes

* Allocation logic was improved - now EasyMAM works correctly with the oldest version of the application (hot detach logic).

## Version 5.20 (19 Nov, 2021)

### Changes

* The logic of splitting positions during the detach is optimized.
* The logic of creating log files was optimized. Now EasyMAM does not generate a huge amount of logs.

## Version 5.19 (17 Nov, 2021)

### Changes

* The bug of hot detach logic was fixed - inner memory storage was improved. 

## Version 5.18 (15 Nov, 2021)

### Changes

* The logic of starting service was improved - several bugs that appeared during the service start were fixed.
* The default settings of EasyMAM were corrected.

## Version 5.17 (11 Nov, 2021)

### Changes

* Inner logic optimization that allows to process large numbers of slave accounts faster.
* RAM usage optimization.

## Version 5.16 (5 Nov, 2021)

### Changes

* Negative stop loss values now are possible to use.

## Version 5.15 (5 Nov, 2021)

### Changes

* An Exception error that occurs when processing a large trading history was fixed.

## Version 5.14 (3 Nov, 2021)

### Changes

* Logic for deals deleting has been optimized. 
* Log files now contain the detailed information about the split of masters’ positions during the hot detach process.
* The logic of the split position (hot detach function) is optimized. 

## Version 5.13 (29 Oct, 2021)

### Changes

* IgnoreOpenTrades bugs are fixed.
* Log file messages are extended.

## Version 5.12 (25 Oct, 2021)

### Changes

* Inner logic optimization: master accounts trading history request is optimized (part 3).
* Orders/deals logic is optimized (part 2).
* IgnoreOpenTrades bugs are fixed.
* Log file messages are extended.

## Version 5.11 (18 Oct, 2021)

### Changes

* Inner logic optimization: master accounts trading history request is optimized (part 2).
* Orders/deals logic is optimized (part 1).
* IgnoreOpenTrades bug is fixed.
* TP/SL now copies to slave orders/deals.

## Version 5.10 (18 Oct, 2021)

### Changes

* Inner logic optimization: master accounts trading history request is optimized (part 2).

## Version 5.09 (17 Oct, 2021)

### Changes

* Hot-detach SL/TP bug fixed.

## Version 5.08 (14 Oct, 2021)

### Changes

* Inner logic optimization: master accounts trading history request is optimized (part 1).

## Version 5.04 (08 Oct, 2021)

### Changes

* Expert ID field is copied to slave accounts’ deals.
* Log files messages are extended.

## Version 5.01 (23 Sep, 2021)

### Changes

* Added fatal login error when 2 trades of the slave have a comment that matches the parent trade of the master.

## Version 4.08 (23 Sep, 2021)

### Changes

* Bug with the creation of additional tabs "other users" after detach slaves from master was fixed.
* User list resync is added.

## Version 4.15 (17 Sep, 2021)

### Changes

* Added fatal log on error when 2 trades of the slave have a comment that matches the parent trade of the master.

## Version 4.13 (23 Aug, 2021)

### Changes

* Masks were cut off by 128 symbols and the bug was fixed.

## Version 4.12 (6 Aug, 2021)

### Changes

* The minor connection bugs are fixed (data transfer between EasyMAM application and TPT License server is improved).
* The minor bugs of logging are fixed.

## Version 4.10 (2 Aug, 2021)

### Changes

* The information about incorrect slave balances is added to the log file.

## Version 4.03 (21 Jun, 2021)

### Changes

* Inner memory bug is fixed.
* The bundle is made as one .exe file (instead of many different files).
* Data type conversion bug is fixed.
* The information about balances and equity of slave accounts is added to log files.
* The detection of incorrect routing rule for Dummy account is added.

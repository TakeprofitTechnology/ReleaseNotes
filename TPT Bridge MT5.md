# Takeprofit Bridge MT5

## Version 25.11.27.49 (1 December, 2025)
### Changes
* Extra Slippage can now be applied with actions H and HM even with Delay=0.

## Version 25.11.20.18 (20 November, 2025)
### Changes
* .xml, .csv files have been replaced with new formats for backup compatibility.
* Overall logging improvements: server/owner name is now stored to cache on first gateway start.
* FATALs are now can be sent before actual gateway start (on initialization process).

## Version v25.10.23.46 (27 October, 2025)
### Changes
* Processing of REST API requests have been rebuilt.

## Version 25.10.01.52 (1 October, 2025)
### Features
* 'Zip' is added to the Rules.
* Basic settings have been updated on first gateway run.

## Version 25.09.26.42 (30 September, 2025)
### Changes
* Log messages have been improved for better understanding.

## Version 25.09.25.46 (25 September, 2025)
### Changes
* Added sending of group owners info to the Report server.

## Version 25.09.15.37 (15 September, 2025)
### Features
* 'Send test trade' added to 'Tools'.

## Version 25.09.01.46 (1 September, 2025)
### Changes
* 'Country' is added to the Rules.

## Version 25.08.26.65 (26 August, 2025)
### Changes
* Fixed an issue with order execution by old price in FillUsingOrderBook mode.

## Version 25.08.15.37 (19 August, 2025)
### Changes
* Changed license name to Takeprofit Bridge MT5.

## Version 25.08.13.52 (14 August, 2025)
### Changes
* Fixed issue with Bridge did not start after MT server restart. 

## Version 25.07.22.43 (22 July, 2025)
### Changes
* The bug of incorrect VWAP price definition is fixed.

## Version 25.07.21.38 (21 July, 2025)
### Changes
* Validation that prevents incorrect symbols in slippage fields is added.

## Version 25.07.03.67 (3 July, 2025)
### Changes
* Internal adjustments of the product (restrictions from 'cut' version are now put on gateway level);

## Version 25.06.30.24 (30 June, 2025)
### Features
* Added the 'cut' version of TPT Bridge, which is managed via License file;
### Changes
* Added support of QUIK connector.
* Added 'Account color' parameter to the rules.

## Version 25.06.10.59 (10 June, 2025)
### Changes
* Fixed a bug when external data was not sent to LP with default rule with H mode;

## Version 25.05.30.45 (30 May, 2025)
### Changes
* The gateway will be automatically started if it is down accidently.
* Added log messages when the gateway cannot connect to the server with manager API.

## Version 25.05.28.39 (25 May, 2025)
### Changes
* Added support of Cyrillic symbols in license name. 

## Version 25.05.16.59 (16 May, 2025)
### Changes
* Fixed Bridge falling down with fatal, now it returns an error to GUI and writes an error message to log;

## Version 25.05.09.38 (9 May, 2025)
### Changes
* Fixed a fatal bug with gateway crash on rare SlippageTolerance values;

## Version 25.04.30.48 (30 April, 2025)
### Features
* Actions SM and HM has been added;

## Version 25.04.21.59 (21 April, 2025)
### Changes
* 'Reason' filter in Rules has been redesigned;

## Version 25.04.08.61 (8 April, 2025)
### Changes
* Corrected m1 filling behavior for action W if UseMT5Quotes is true;

## Version 25.04.02.40 (2 April, 2025)
### Changes
* External data (FIX) is extended: now Kloshira passes the volume step of the traded symbol.
### Features
* The gateway now can perform the B-book reports.

## Version 25.03.19.46 (19 March, 2025)
### Changes
* Added a fatal message to logs in case manager connection is failed on start;

## Version v25.03.11.68 (11 March, 2025)
### Features
* New slippage values added to execution report;

## Version v25.02.19.52 (19 February, 2025)
### Changes
* Server type is added to JSON external data of FIX messages;

## Version v25.02.17.44 (17 February, 2025)
### Changes
* Improved logging on shutdown;

## Version v25.02.13.46 (13 February, 2025)
### Changes
* Symbols are now processed automatically for B-book modes;
* MT API Update;

## Version v25.01.31.51 (31 January, 2025)
### Changes
* Server name is added to JSON external data of FIX messages;

## Version 25.01.27.61 (27 January, 2025)
### Changes
* Logging bug is fixed.

## Version 25.01.23.35 (23 January, 2025)
### Changes
* Fixed bug with Manager API reconnection;

## Version 25.01.21.46 (21 January, 2025)
### Changes
* Minor changes in log messages; 

## Version 24.12.24.47 (24 December, 2024)
### Features
* Unsupported parameters are now displayed in log file;

## Version 24.12.18.52 (18 December, 2024)
### Changes
* The gateway sync timeout on restart has been increased; 

## Version 24.12.13.39 (13 December, 2024)
### Changes
* REST strings have been removed from logs;

## Version 24.12.09.79 (9 December, 2024)
### Changes
* MT5 Gateway API has been updated to v4731;

## Version 24.12.02.36 (2 December, 2024)
### Changes
* The logic to connect to any possible access server (if the specified access server is not available) is added.

## Version 24.11.26.44 (26 November, 2024)
### Changes
* Fixed an issue with spread not getting current market value

## Version 24.11.06.39 (06 November, 2024)
### Changes
* Auto sending of users' configuration files for backup is implemented;

## Version 24.10.24.61 (24 October, 2024)
### Changes
* PrimeXM maker connection is improved.

## Version 24.08.13.49 (24 August, 2024)
### Changes
* The log lines that are not needed were removed from log files.

## Version 24.07.31.47 (31 July, 2024)
### Changes
* Bug of incorrect price representation in the GUI is fixed.

## Version 24.07.15.53 (15 July, 2024)
### Changes
* Incorrectly named column in Symbols.csv has been fixed.

## Version 24.06.26.69 (26 June, 2024)
### Changes
* Removed TradingManagers parameter;
* Assymetric negative markups have been fixed.

## Version 24.06.19.48 (19 June, 2024)
### Changes
* Fixed ignoring symbols with # in the beginning of a symbol.

## Version 24.06.11.56 (11 June, 2024)
### Changes
* Fixed folders structure.

## Version 24.05.31.23 (31 May, 2024)
### Changes
* MT5 TPT Bridge for builds 3550 assembled.
* VWAP prices have been rounded.

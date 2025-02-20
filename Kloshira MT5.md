# Kloshira MT5

## Version v25.02.19.52 (19 February, 2025)
### Changes
* Server type is added to JSON external data of FIX messages;

## Verson v25.02.14.73 (14 February, 2025)
### Changes
* API has been updated;

## Version v25.01.31.51 (31 January, 2025)
### Changes
* Server name is added to JSON external data of FIX messages;

## Version v25.01.23.35 (23 January, 2025)
### Changes
* Fixed bug with Manager API reconnection;

## Version v25.01.21.46 (21 January, 2025)
### Changes
* Minor changes in log messages; 

## Version v24.12.24.47 (24 December, 2024)
### Features
* Unsupported parameters are now displayed in log file;

## Version v24.12.18.52 (18 December, 2024)
## Changes
* The gateway sync timeout on restart has been increased; 

## Version v24.12.10.45 (10 December, 2024)
### Changes
* MT5 Gateway API has been updated to v4731;

## Version v24.11.28.42
### Changes
Fixed an issue with spread not getting current market value

## Version v24.09.18.45 (18 September, 2024)
### Changes
* Gateway starting process has been improved to avoid issues inside Gateway API

## **Version 24.06.20.86 (1 June, 2024)**
### Changes
* The bug where the number of digits was not displayed correctly in opened positions that were opened with VWAP price.

## **Version 1.97 (11 December, 2023)**
### Changes
* Added calculation of VWAP for m0 if FillUsingOrderBook=true.

## **Version 1.94-1.95 (14 November, 2023)**
### Changes
* Rebuilt a mechanism of price definition for B-book. Now Kloshira uses the full book insted of the top of the book.
* Added "FillUsingOrderBook" parameter to use the full book.
* Fixed copying deals to the coverage account with wrong symbols during the simultaneous execution.
* Fixed the logs folder path.
* Bug fixed: incorrect execution of SELL orders, execution occurred at the ask price instead of the bid price.

## **Version 1.91 - 1.93 (01 August - 25 September, 2023)**
### Changes
* Kloshira was rebuilt several times with the lates MT5 Gateway API to match the latest version of MT5 server.
* Logging is improved.

## **Version 1.90 (21 July, 2023)**
### Changes
* Added "SubscribeToIncrementalUpdates" parameter to Sessions.ini.

## **Version 1.89 (3 July, 2023)**
### Changes
* Fixed action M bug (min lot in symbol's settings was ignored).
  
## **Version 1.87 (17 March, 2023)**
### Changes
* Fixed NONE reason on closing order closing deals.

## **Version 1.86 (15 March, 2023)**
### Changes
* ‘Receive buffer is too small’ warning moved from trace layer to error.
* Extra delay bug fixed.

## **Version 1.84 (03 March, 2023)**
### Changes
* Bug fixed: wrong sequence number after restart.

## **Version 1.83 (09 February, 2023)**
### Changes
* Added symbol name in error log if configuration of this symbol incorrect.

## **Version 1.82 (23 January, 2023)**
### Changes
* Added milliseconds displaying to quote ticks time.

## **Version 1.81 (01 December, 2022)**
### Changes
* Fixed order execution in case of no quotes and UseMT5Quotes=true.

## **Version 1.79 (01 November, 2022)**
### Changes
* Added execution of limit order as market if X or M actions have negative value.

## **Version 1.77 (06 October, 2022)**
### Changes
* Gateway API updated.
* Added host validation without protocol type.

## **Version 1.74 (07 September, 2022)**
### Changes
* Fixed Gateway crash bug if the routing group name has a % sign in it.

## **Version 1.73 (29 August, 2022)**
### Changes
* Removed stack trace on MT5 Kloshira GUI connection error.

## **Version 1.72 (08 July, 2022)**
### Changes
* Added to logs retcode from DealerStart().

## **Version 1.69 (05 May, 2022)**
### Changes
* In Kloshira, GUI added the ability to leave LP Names field empty.

## **Version 1.68 (19 April, 2022)**
### Changes
* Added the logic to process TA_STOPOUT_ORDER request for a limit order. The limit order is closed in case of reaching the SO level on the trading account. In previous versions, the limit order was not closed by SO.

## **Version 1.67 (15 April, 2022)**
### Changes
* The name of the gateway instance has been added to the logging.

## **Version 1.66 (12 April, 2022)**
### Changes
* The name of filtering quotes with zero spread has been changed to ZeroSpreadFilterWidthPercent.

## **Version 1.65 (10 April, 2022)**
### Changes
* Added filtering of quotes with zero spread, ZeroSpreadFiltrationWidthPercent.

## **Version 1.64 (01 April, 2022)**
### Changes
* Changed the error text when entering values in the Schedule field incorrectly.

## **Version 1.63 (09 March, 2022)**
### Changes
* Added Security column to the new Kloshira Web GUI.
* Fixed bug, the Balance Kloshira Web GUI field accepts any values.

## **Version 1.62 (20 January, 2022)**
### Changes
* The unexecuted part is not cancelled during limit order execution.

## **Version 1.61 (20 January, 2022)**
### Changes
* The unexecuted part is not cancelled during limit order execution.
* Additional logging information was added for the case: manager account is not set (MT5 Administrator).

## **Version 1.59 (23 November, 2021)**
### Changes
* “SubAccount” parameter was deleted from the rules in GUI.

## **Version 1.58 (23 November, 2021)**
### Changes
* Gateway was completely reassembled with a new version of manager API.

## **Version 1.57 (27 October, 2021)**
### Changes
* Added value “{details}” for in the parameter “newSubaccount” of the routing rule for displaying detailed information in the FIX logs.

## **Version 1.56 (28 September, 2021)**
### Changes
* Fixed a bug, when using a domain in the gateway parameters, it did not start.
* Added a message to the logs when using a domain name in parameters.

## **Version 1.55 (26 September, 2021)**
### Changes
* Rejecting 4 unsupported operation types (Price, Request, Instant, Exchange) was realized.
* Pending orders activation by the manager was fixed.
* Stop limit buy/sell orders were fixed.
* Logging was improved. Added information about unsupported operation types: name of request type and order type.

## **Version 1.54 (15 September, 2021)**
### Changes
* Changed the text of the fatal log in which If an active order was being processed on the trading account at the time the gateway was restarted.

## **Version 1.53 (15 September, 2021)**
### Changes
* If an active order was being processed on the trading account at the time the gateway was restarted, a fatal message is displayed in the logs.

## **Version 1.52 (08 September, 2021)**
### Changes
* Bug has been fixed: when changing the ‘Action” rule, Kloshira stopped working and was dispalyed in the logs fatal exception.

## **Version 1.51 (06 September, 2021)**
### Changes
* Gateway completely rebuilt with new libraries and relieved of dependencies.

## **Version 1.49 (29 June, 2021)**
### Changes
* Action X now can take negative values (in this case the direction of the order will be changed).
* Action M now can take negative values (in this case the direction of the order will be changed).

# Kloshira MT4

## Version v24.09.20.46 (20 September, 2024)
## Changes
* Slippage is now applied when Delay is 0; 

## Version 24.09.02.45 (09 August, 2024)
### Changes
* AllowVWAPPrice bug is fixed (the logic of this parameter was not working correct).

## Version 4.30 (21 September, 2023)
### Changes
* Added check for logQuote.
* "std::format" to compile log messages is used now.
* Refactored quotes handling in FIX Acceptor.

## **Version 4.30 (29 August, 2023)**
### Changes
* Code optimization was made.
* "Receive buffer is too small" was changed from ERROR to INFO message.

## **Version 4.27 (22 August, 2023)**
### Changes
* Optimized quote processing for speeding up.

## **Version 4.24-4.26 (09 June, 2023)**
### Changes
* Optimization changes. Internal logic of delivering quotes to MT4 was changed.

## **Version 4.23 (14 March, 2023)**
### Changes
* ‘Receive buffer is too small’ warning moved from trace layer to error.

## **Version 4.22 (11 March, 2023)**
### Changes
* Added SkipServerValidation setting to Kloshira.

## **Version 4.21 (10 March, 2023)**
### Changes
* Added TradeUpdatesInThreadPool setting to Kloshira.

## **Version 4.20 (05 March, 2023)**
### Changes
* Optimized server validation process.

## **Version 4.19 (10 February, 2023)**
### Changes
* Removed checking parameters of Security in case of disabled Trading for Securities.


## **Version 4.18 (29 December, 2022)**
### Changes
* Added REST API command to restart fix.
* Added REST API command to set symbols.
* Added REST API command to get symbols.
* Added REST API command to reload symbols.

## **Version 4.17 (20 December, 2022)**
### Changes
* Code optimization made.

## **Version 4.16 (16 September, 2022)**
### Changes
* Added execution of limit order as market if X or M actions have negative value.

## **Version 4.12 (06 May, 2022)**
### Changes
* Negative slippage could be set with limit orders now.
* LockManagerOrders parameter was added to the plugin settings.

## **Version 4.10 (06 April, 2022)**
### Changes
* The setting ZeroSpreadFiltrationWidthPercent changed to ZeroSpreadFilterWidthPercent, working logic the same.

## **Version 4.09 (05 April, 2022)**
### Changes
* The ZeroSpreadFiltrationWidthPercent setting was added to filter the quotes with zero spread.

## **Version 4.08 (17 January, 2022)**
### Changes
* Fixed critical error text when entering wrong port in ClientSessions. Fixed to “FIX Acceptor can't use the specified port. Please check if the specified port is not busy or define another port.
* Changed message in the log about WVAP calculation.

## **Version 4.07 (17 January, 2022)**
### Changes
* FXOPEN connector is now getting the quotes for more than one symbol without rejects.

## **Version 4.06 (21 December, 2021)**
### Changes
* “AllowVWAPPrice” parameter was added. This parameter allows you to calculate the b-book part of the transaction at the weighted average price in action “M” and “X”.
* Minor loggin improvements: symbol displayed without quotes in “error” or “warning” messages in log files.
* CFH, FXALLBSSSP2, FXOPEN connectors were fixed.
* FXOPEN connector is now getting the quotes for more than one symbol without rejects.

## **Version 4.05 (01 December, 2021)**
### Changes
* Added support for limit orders in the BYFX connector.

## **Version 4.04 (17 November, 2021)**
### Changes
* Fixed GUI bug, related to Metatrader API crash when receiving email notification.
* Adjusted PumpingSwitch “CLIENT_FLAGS_HIDEMALL” parameter in the code.

## **Version 4.03 (27 October, 2021)**
### Changes
* The log when used tick logging for symbols is now displayed as an info message.
* The log when used Smoothing for symbols is now displayed as an info message.
* Added value “{details}” for in the parameter “newSubaccount” of the routing rule for displaying detailed information in the FIX logs.

## **Version 4.02 (21 September, 2021)**
### Changes
* Added FOK to OneZero connector.

## **Version 4.01 (08 September, 2021)**
### Changes
* Bug fixed - Kloshira MT4 does not allow preserving the A-Book routing rule.
* Bug fixed - Fatal error when deleting A-Book routing rule.



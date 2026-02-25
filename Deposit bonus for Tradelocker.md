# Deposit bonus for Tradelocker


## Version 2026.2.20.576 (20 February, 2026)
### Changes
* Websocket API is removed.
* Requesting accounts states via REST API.
* Check of missing operations is removed.

## Version 2026.2.1.1089 (2 February, 2026)
### Changes
* The bug (the bonus is not deducted when ev < bonus amount) is fixed.

## Version 2026.1.29.363 (29 January, 2026)
### Changes
* Now the application processes bonuses and withdrawals according to their order (first in - first processed).


## Version 2025.12.29.587 (29 December, 2025)
### Changes
* Second part of inner optimizations and refactoring. The speed of bonus processing is increased.


## Version 2025.12.23.3820 (23 December, 2025)
### Changes
* Inner optimizations and refactoring. The speed of bonus processing is increased.

## Version 2025.12.19.710 (19 December, 2025)
### Features
* The app removes the bonus if equity is less than bonus amount.
### Changes
* Tooltips are removed from the GUI.
* The parameter "ApiRateLimitPer10Sec" is added to the application.

## Version 2025.12.15.416 (15 December, 2025)
### Features
* Max bonus (acc ccy) parameter is added (the parameter allows to set max bonus amount for one bonus).
* Bonus withdrawal logic is added.
### Changes
* Bonus rules are added to log files.

## Version 2025.12.9.653 (9 December, 2025)
### Features
* The logic of total bonus for each account is added.
### Changes
* The license check mechanism is added.

## Version 2025.12.8.985 (8 December, 2025)
### Changes
* REST API requests are now added to log files.
* The logic of bonus creation is added (as a credit and as a deposit).

## Version 2025.12.2.742 (2 December, 2025)
### Changes
* GUI is created.
* Rules saving and editing logic is added.
* appsettings.json file with parameters is added.
* REST API integration with Tradelocker is added.
* The logic of deposit tracking is added.


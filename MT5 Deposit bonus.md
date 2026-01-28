# MT5 Deposit Bonus

## Version 26.01.15.77 (20 January, 2026)
### Changes
* Minor internal optimizations and stability improvements have been implemented.

## Version 25.11.24.63 (16 December, 2025)
### Changes
* Fixed the rounding issue which blocked withdrawal of funds in some cases.

## Version 25.10.10.54 (10 October, 2025)
### Changes
* Cache initialization has been improved:
Optimized data loading.
Skip cache rebuilding on settings change if affected groups aren't changed.
Fixed long plugin shutdown when cache is recalculated.
* Fixed negative credit after bonus deduction.
* Fixed withdrawal blocking logic: skip credit out operations.

## Version 25.10.07.40 (7 October, 2025)
### Changes
* Improved caching process which lead previously to server freezes.

## Version 25.10.01.33 (1 October, 2025)
### Changes
* Fixed creation of zero balance operation is some cases.
* Added a check for the user's current credit state in the withdrawal logic to prevent deducting already deducted credit. 

## Version 25.08.22.58 (26 August, 2025)
### Features
* CreditRemovalOnBalanceLossPercent parameter has been added.

## Version 25.08.08.44 (11 August, 2025)
### Changes
* Fixed an issue when SO triggerring did not lead to credits deduction. Now when SO is triggered, plugin deduct credits correctly.
### Features
* EqualizeCreditDownToBalanceOnWithdrawal parameter has been added;

## Version 25.07.30.59 (31 July. 2025)
### Changes
* Fixed a bug with 'CreditExpirationDays' led to fatal if not specified correctly;

## Version 25.07.18.56 (18 July, 2025)
### Changes
* Fixed duplicating credit charging.

## Version 25.07.15.49 (25 July, 2025)
### Changes
* The parameter "CreditDrawdownPercent" is added to the plugin.
* The parameter "CreditExpirationDays" is added to the plugin.

## Version 24.08.20.50 (21 August, 2024)
### Changes
* A new parameter 'RemoveCreditOnWithdrawal' has been added, allowing users to deduct credit balance when the trading account performs a withdrawal operation;

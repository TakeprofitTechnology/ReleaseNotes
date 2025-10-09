# MT5 Deposit Bonus

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

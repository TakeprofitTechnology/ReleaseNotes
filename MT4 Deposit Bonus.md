# MT4 Deposit Bonus

## Version 26.09.22.31 (28 September, 2026)
### Changes
* Fixed withdrawals taking out more bonus credit than the plugin had issued. This could leave the account with negative credit.
* A withdrawal no longer creates a credit order when the account has no bonus credit left.
* Operations on the same account are now always processed one by one, in order. This stops the same credit from being deducted twice.
* Accounts that already have negative credit are not fixed automatically. The next deposit's bonus covers the negative amount first. To fix an account right away, delete the wrong negative credit order from its history.

## Version 25.10.14.27 (14 October, 2025)
### Changes
* Fixed the issue when the plugin settings were not updated until server restart.

## Version 25.10.01.33
### Changes
* Fixed creation of zero balance operation is some cases.

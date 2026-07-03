# Auto Hedger MT5


## Version 26.06.30.22 (30 June, 2026)
### Changes
* Fixed a bug where a failed REST bind on first load could deadlock the entire MT5 trade server.
### Features
* Added an optional "Account Color" filter to hedging rules — a rule can now apply only to accounts with specific standard MT5 colors, matching the existing behavior in TPT Bridge and Hub. Custom colors are not supported, and rules without a color set continue to apply to all accounts as before.

## Version 26.06.01.46 (4 June, 2026)
### Changes
* Fixed the error messages shown when the plugin cannot interpret an order on the omnibus account to now include an explicit hint that trade accounts must not belong to an omnibus group.
## Version 26.04.09.47 (15 April, 2026)
### Changes
* OmniGroups parameter has been added. Now it's possible to specify multiple omnibus accounts for the plugin work.
* Now it is possible to trigger multiple rules at once - they are not working in terms of priority.

## Version 2026.3.5.724 (6 March, 2026)
### Changes
* Fixed the WebGUI bug with stuck cells.

## Version 26.02.23.52 (24 February, 2026)
### Changes
* History page has been added.
* Comment format has been changed.
* Fixed the bug with deals being duplicated on coverage account.

## Version 26.01.22.46 (22 January, 2026)
### Changes
* Initial plugin version has been released.
* The rejection mechanism for pending orders has been amended. If the plugin cannot open a pending order due to the 'Invalid price' rejection reason from MetaTrader, the market order will be opened instead.

# Broctagon Risk Panel

## Version 2026.9.22.641 (22 September, 2026)
### Features
* Added the Equity coverage alert page. When a client's Hub equity falls below MT5 equity by more than the set tolerance, the panel sends a notification through a make.com webhook.
* The alert tolerance can be set in USD, in percent, or both. Cooldown and escalation settings control repeat notifications.
* Added a Settings button to the Balances page to change the highlight thresholds: the balance buffer in USD and the equity difference in percent. Defaults stay 10 000 USD and 10%.
* Each highlight rule can now be turned off. The page shows the current thresholds and how many rows are highlighted.
### Changes
* Fixed table data overlapping the header on the Positions page.
* The panel has a new interface. Addresses, logins and columns stay the same.
* Data now appears about 40 seconds after start instead of about 5 minutes. Balances refresh every minute, positions every 5 minutes.
* Each page shows how old its data is. A source that does not answer is shown as unavailable, not as zero.
## Version 2026.9.9.618 (9 September, 2026)
* Added equity comparison to the Balances page, showing MT5 and Hub equity and highlighting differences of 10% or more.

## Version 2026.9.7.760 (8 September, 2026)
### Changes
* The panel can now collect data from several OneZero databases at once. The single `DatabaseConnectionId` setting in the `OneZeroSettings` section has been replaced with the `DatabaseConnectionIds` list, for example: `"DatabaseConnectionIds": [ 4275, 8374 ]`.
* This fixes the discrepancies in positions that appeared after OneZero archived a part of its data: the panel used to read the live database only. When a new archive appears, it is enough to add its connection ID to the list.
## Version 2026.6.29.789 (1 July, 2026)
### Changes
* Removed the MT4 server entirely from the panel, as it's no longer used in the client's setup.

## Version 2026.5.22.708 (26 May, 2026)
### Changes
* Memory usage overall optimisation.
* Dramatically reduced network activity (~126 KB/sec avg vs ~5 MB/sec avg in old version)
* Significantly lower CPU usage (~1.5% avg vs ~33% avg in old version);

## Version 2026.5.15.562 (21 May, 2026)
### Changes
* OZ BP Total column has been added.

## Version 2026.4.29.497 (30 April, 2026)
### Changes
* Now it's possible to copy info from Balances to buffer.
* Added Broctagon Hub 2 column.
* Changed the logic of difference highlightning. Now it works this way: (Hub balance + credit + 10000 USD) - (DC balance + credit) = if the difference is below 10000 → highlight in red.

## Version 2026.4.10.626 (10 April, 2026)
### Changes
* Added sorting to columns in Balances menu.
* OneZero TOTAL column has been removed.
* Added filter for 'Dropcopy accounts' section.
* Logging has been improved.

## Version 2026.3.26.785 (3 April, 2026)
### Changes
* MT4/5 DC Sum columns have been reverted.
* GL section has been removed.

## Version 2026.2.27.565 (6 March, 2026)
### Changes
* Fixed the mapping mechanism. Added logging for $BRO symbols mapping.

## Version 2026.2.17.891 (20 February, 2026)
### Changes
* Fixed the logic of auto defining the list of dropcopy accounts: GL & FXGrow accounts are excluded.
* Added 'Coverage on Broctagon' column for positions on Broctagon hub.

## Version 2026.2.2.381 (2 February, 2026)
### Changes
* FXGrow part has been removed from the panel.

## Version 2026.1.16.585 (22 January, 2026)
### Changes
* Two new columns have been added to the FX Grow section: “Secondary FX Grow hub” and “OZ BP 2 Secondary"
* OZ connection has been fixed.

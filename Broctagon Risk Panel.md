# Broctagon Risk Panel

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

# NOP limit MT5

## Version 26.09.21.31 (25 September, 2026)
### Changes
* The plugin now refuses to start if a setting or limits file is missing or invalid. The Administrator shows a red "DISABLED" status with the reason.
* A bad configuration pushed while the plugin is running is now rejected. The previous limits stay in effect, and the MT5 server never needs a restart.
* Limit files now reject impossible values, such as negative limits, text in number fields or unknown values in the Enabled column. The error names the file, column, line and value. Check your limit files before upgrading.
* Orders that are accepted but not yet filled now count toward the account limit.
* Repeated server errors now appear in the journal as one summary line per minute.

## Version 26.03.02.44 (3 March, 2026)
### Changes
* Added virtual position cache to reduce execution delays.

## Version 26.01.29.54 (3 February, 2026)
### Changes
* Fixed the rounding issue which triggered the plugin to block the volume even if the threshold is not reached.

## Version 25.11.24.64 (24 November, 2025)
### Changes
* Added 'PASSED' event to log files.

## Version 25.10.28.51 (30 October, 2025)
### Features
* 'Volume unit' parameter has been added to define how limit will be calculated: in lots or in USD.

## Version 25.07.22.64 (22 July, 2025)
### Changes
* Added "Enabled" option to each NOP rule to enable/disable it.

## Version 25.04.11.52 (11 April, 2025)
### Changes
* Fixed operation of RuleLogins cache inside the plugin;
* Fixed the logic of the plugin with rules where the same users are present;
* Fixed spamming of plugin cache update logs on events of changing or adding all accounts on the server;
* Improved logging;

## Version 25.04.10.32 (10 April, 2025)
### Changes
* Fixed a bug in calculating the current NOP in USD for Forex symbols; 

## Version 25.03.18.48 (18 March, 2025)
### Changes
* The bug with incorrect calculation of commissions, when account currency was USD, has been fixed;

## Version 25.03.05.44 (5 of March, 2025)
### Changes
* BUG fixed: it was possible to exceed the limits using TP orders.

## Version 25.03.03.47 (3 of March, 2025)
### Changes
* Shared accounts volume feature is added to the pluign.

## Version 25.02.19.51 (19 of February, 2025)
### Changes
* BUG fixed: incorrect calculation of volume for futures.


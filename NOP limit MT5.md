# NOP limit MT5

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


# MT4 Swap Control Center


## Version 26.11.17.42 (17 November, 2026)
* Fixed accumulated swaps not being charged when AccumulateCharge is enabled with SwapType=SWAP.
* Improved accumulated swap handling to prevent lost or duplicate charges during rollovers.
* Improved error logging for failed balance operations, including the amount, order, and login.

## Version 26.10.26.61 (28 October, 2026)
### Changes
* Updated third-party libraries to their latest stable versions.
* Empty groups and symbol swaps lists now show as empty in the configurator. Before, they caused an error.
* A volume limit of 0.29 lot is now read exactly. Before, it was read as 0.28 lot.

# TL Deposit bonus

## Version 2026.4.2.950 (2 April, 2026)
### Changes
* Reduced plugin startup delay (~13 → ~3.5 min) by skipping unnecessary account discovery on first bonus check and significantly cutting API calls.
* Fixed excessive logging and added cleanup for stuck pending operations (>24h), improving stability and processing reliability.

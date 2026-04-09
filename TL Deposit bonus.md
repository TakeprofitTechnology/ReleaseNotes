# TL Deposit bonus

## Version 2026.4.2.950 (2 April, 2026)
### Changes
* Reduced plugin startup delay (~13 → ~3.5 min) by skipping unnecessary account discovery on first bonus check and significantly cutting API calls.
* Fixed excessive logging and added cleanup for stuck pending operations (>24h), improving stability and processing reliability.

## Version 2026.3.30.582 (30 March, 2026)
### Changes
* Fixed lost bonuses during rule changes by introducing rule history, ensuring deposits receive the correct bonus based on the active rule at deposit time.
* Added fast-track account discovery (reducing delay to ~5s) and expanded test coverage (45+ tests) to improve reliability across rule changes and edge cases.
* Implemented structured logging for skipped bonuses ([-BONUS_REPORT]) with clear reason codes, reduced log spam, and improved visibility (account IDs, summaries, shutdown logs).
* Fixed logging issues (null fields removed) and enhanced observability of bonus processing and system behavior.

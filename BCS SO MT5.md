# BCS SO MT5

## 26.06.01.57 (5 June, 2026)
### Changes
* The stop-out comment now reflects the actual margin level at which the stop-out was triggered. If the trigger level was below MinimumMarginLevel, the comment shows MinimumMarginLevel instead.
* Fixed a bug where a position could be adjusted twice and another one skipped when the stop-out-triggering position was not the first to be closed.
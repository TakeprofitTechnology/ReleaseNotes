# MT5 Deal bid - ask recorder

## Version 26.10.16.15 (21 October, 2026)
### Changes
* Logging now uses our own logger instead of a third-party library. Log files, names, rotation and line format stay the same.
* Log lines now reach the log file almost at once. Before, they could be up to 30 seconds late.
* The plugin no longer waits more than 5 seconds for a log line, so a slow or stuck disk can't freeze it.
* If the process is killed, the last log lines are no longer cut off.

## Version 26.10.08.49 (8 October, 2026)
### Changes
* Fixed the plugin freezing and no longer recording deals under heavy load.

## Version 1.01-1.03 (October 2021 - February 2023)
### Changes
* Minor changes to fit the code base.

## Version 1.0 (23 October, 2020)
* Initial version of the plugin has been released.

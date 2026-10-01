# Takeprofit MarketDepth MT5

## Version 26.09.28.39 (28 September, 2026)
### Features
* The gateway was rewritten in C++. It uses several times less processor time per price update and less memory than the previous version.
* One gateway can now serve the symbols that used to be split across several gateways, so the MT5 server no longer receives duplicate order book updates.
* Added a migration tool that converts existing gateway records into one configuration. If two records set up the same symbol differently, it stops and explains the conflict.
* Added configuration through the Web GUI configurator (EnableGUIConfiguration). Changes take effect on the running gateway without a restart, and a change with errors is refused as a whole with every reason listed.
* A new Web GUI mode record now gets starter Settings.ini and SymbolBooks.dat files and listens on 127.0.0.1, port 1975 by default.
* A symbol entry can now be a pattern: a star matches any characters, terms are separated by commas, and a term starting with "!" excludes symbols. An exact entry placed above a pattern keeps its own settings.
* A symbol can now be set to no feed, so its depth is built only from the pending orders of the broker's clients.
* The gateway now checks its manager rights after connecting. If a right is missing, it switches the client order feature off and names the missing rights in the log.
* The gateway now names the symbols whose depth the MT5 server discards, for example symbols that copy prices from another symbol.
* The settings the gateway read are now written to the main log at start. Passwords are never included.
### Changes
* The connection status no longer shows the gateway as connected when all price feeds are down or nothing is being published.
* Feed passwords are no longer written to the logs.
* Symbols whose name at the price feed differs from the MT5 name are now published.
* Trade requests are no longer left unanswered until the server times out.
* The order book no longer shows the same price on both sides or more levels than the symbol allows.
* Client orders are removed from the book when the manager connection drops.
* Fixed a limit order with the Return fill policy losing volume or getting stuck after partial fills.
* A start refused because of settings errors no longer repeats the full error list on every restart.
* Old settings left on a Web GUI mode record in the MT5 Administrator are now ignored instead of blocking the start.
* A feed connection that failed to start is now restarted by the next saved configuration change.
* The gateway no longer creates an empty "fix" folder in its logs.

## Version v2024.12.10.1324 (10 December, 2024)
### Changes
* The gateway is rebuild using the latest version of gateway API (5120).

## Version v2024.12.10.1324 (10 December, 2024)
### Changes
* MT5 Gateway API has been updated to v4731.

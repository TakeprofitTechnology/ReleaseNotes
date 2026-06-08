# Price Monitoring Tool MT4

## Version v2026.6.5.579 (5 June, 2026)
### Changes
* Alert titles now display the server alias from appsettings.json when the MT4 server is unavailable at startup, instead of showing an empty title.
* Fixed alert titles becoming empty in additional scenarios where server name information was missing during reconnect.


## Version v2024.12.23.928 (23 December, 2024)
### Changes
* SendErrorExpirationTimeInMinutes parameter now aggregates exceptions into 1 message;

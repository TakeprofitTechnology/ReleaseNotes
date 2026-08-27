# Price Monitoring Tool MT4


## Version 2026.8.26.435 (26 August, 2026)
* Deleted MT4 symbols now stop being monitored within one minute, preventing false price alerts.
* Symbol status changes are now clearly reported in the logs.


## Version 2026.8.19.982 (19 August, 2026)
* Improved market-hours monitoring with correct handling of closed, overnight, consecutive and overlapping quote sessions, faster schedule updates, and more reliable monitoring and alert recovery.


## Version 2026.6.5.579 (5 June, 2026)
### Changes
* Alert titles now display the server alias from appsettings.json when the MT4 server is unavailable at startup, instead of showing an empty title.
* Fixed alert titles becoming empty in additional scenarios where server name information was missing during reconnect.


## Version 2024.12.23.928 (23 December, 2024)
### Changes
* SendErrorExpirationTimeInMinutes parameter now aggregates exceptions into 1 message;

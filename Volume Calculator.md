# Volume Calculator

## Version 2026.7.31.67 (31 July, 2026)
### Changes
* Speeded up report store discovery for large stores — choosing a client with a very large number of stored reports no longer fails with a timeout.
* Removed the selection size limit that rejected wide date ranges with "Selected range is too large to process at once". Reports are now aggregated while the files are read, so a full month of a large client's reports can be calculated in one run.
## Version 2026.7.17.692 (24 July, 2026)
### Features
* Volume Calculator now reads report logs directly from a configured store folder instead of requiring manual log uploads. Pick a client, server and product, set a date range and click Calculate to download a CSV. Configure the source via the new `ReportsFolder` parameter in appsettings.json.

## Version 2025.4.18.736 (18 April, 2025)
### Changes
* Fixed a bug with incorrect market slippage calculation;

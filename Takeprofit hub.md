# Takeprofit hub

## Version 2025.08.22.698 (22 August, 2025)
### Changes
* Fixed the issue when disabled maker sent FIX messages.

## Version 2025.08.19.510 (19 August, 2025)
### Changes
* VULKAN maker type has been added.
* Fixed the issue with order 'Off Quotes' reject when adding symbol through a Price channel.
* Fixed exception on application shutdown.
* Removed the possibility for the user to delete himself.
### Features
* Schedule has been added to Risk profiling rules.
* Reject option has been added to Risk profiling rules.

## Version 2025.08.05.364 (5 August, 2025)
### Changes
* The hub saves price charts to it's database.
* Minor export TSV bugs are fixed.

## Version 2025.08.04.329 (4 August, 2025)
### Changes
* Minor GUI issues are fixed.
* Several parts of code are refactored (minor improvements).

## Version 2025.07.24.651 (24 July, 2025)
### Changes
* The export of Account's positions to TSV file is added.
* Orders table filters are improved (now possible to set several criterias for filtering).
* Added "Inactive" section to Home page.
* Added a possibility to specify the list of makers to price channels rules.

## Version 2025.07.23.291 (23 July, 2025)
### Changes
* Risk management module syncronization is improved.
* Price channels import/export is improved (makers list is added to CSV files).

## Version 2025.07.21.664 (21 July, 2025)
### Changes
* Bug is fixed: it was possible to remove taker even if it was confugured as dropcopy for some other taker.

## Version 2025.07.16.668 (16 July, 2025)
### Changes
* The book representation bug (volumes from all levels are collapsed to the GUI in one sigle level ) for all accounts except admin account is fixed.

## Version 2025.07.09.558 (09 July, 2025)
### Changes
* The width of Takers filed (Risk profiles => Rules) is increased.
* The text of disabled risk management tab in hub's GUI is improved.
* The text of incorrect make.com webhook warning is improved.
* Small improvements for position adjustment (Account => Positions) are added.

## Version 2025.07.03.329 (03 July, 2025)
### Features
* "Dropcopy to taker" is added to takers' settings.
### Changes
* Fixed the bug of incorrect notification representation in Risk management tab.
* Small improvements to makers connection string are added.
* Now it is possible to use spaces in Risk profiles => Rules => External groups.
* "Makers" button is added to Risk profile information page.

## Version 2025.07.01.532 (01 July, 2025)
### Changes
* Fixed a bug with no possibility to put negative values to price channels markups.
### Features
* Added the parameter “Start book from level”.

## Version 2025.06.26.530 (26 June, 2025)
### Changes
* Comment field has been added for Makers, Takers, Price channels.

## Version 2025.06.24.939 (24 June, 2025)
### Changes
* CYSEC report page has been added.
* Risk management panel is now integrated as a separate service.
* The search mechanism is changed, now shows all entities that consist entered symbol.

## Version 2025.06.16.371 (16 June, 2025)
### Changes
* Country field is added to Accounts preferences.
* Added support of MT4 servers for Risk Management panel.
 
## Version 2025.06.06.661 (6 June, 2025)
### Changes
* Daily profit (Risk management) calculation logic is improved.

## Version 2025.06.05.815 (5 June, 2025)
### Changes
* Risk management tab optimization is made: the data retreiving is improved, the resource usage (RAM) is optimized.
* Overall visual improvements of tables in 'Risk management' section.
* The bug of deleting MT servers from the table "MetaTrader servers" is fixed.


## Version 2025.05.28.584 (28 May, 2025)
### Changes
* The chart "Balances and equities" (Risk management tab) is transposed.
* Log level is raised to "FATAL" for error "multiple FIX connection to one FIX session".
* Risk management tabs are refactored and optimized.
* Since this version it is not possible to change the currency of existing margin account.


## Version 2025.05.27.1244 (27 May, 2025)
### Changes
* Some GUI improvements for Risk management tab are made.

## Version 2025.05.22.305 (22 May, 2025)
### Changes
* Bug fixed: incorrect volume calculation for MT trading accounts in Risk management tab.
### Features
* Now it is possible to override default account with another account in the Rules (Risk profiles).

## Version 2025.05.05.1061 (5 May, 2025)
### Changes
* ResetOnLogon takers logic is improved (OneZero acceptor FIX connection).

## Version 2025.04.28.529 (28 April, 2025)
### Changes
* Minor GUI improvements in "Risk management" & "Risk profiles";
* "Accounts" filter is improved.

## Version 2025.04.21.660 (21 April, 2025)
### Changes
* Fixed a bug with server saving without specifying the server type;
* GUI improvements in 'Risk management' tab.
### Features
* 'Servers' filter has been added to the filter list of 'Daily data';
* 'Change price' feature has been added to 'Risk profiles' > 'Rules';
* 'Account's volumes' has been added to Risk management;
* 'Winners/losers' has been added to Risk management.

## Version 2025.04.11.488 (11 April, 2025)
### Changes
* Some minor GUI improvements (Risk profiles => Rules).

## Version 2025.04.10.493 (10 April, 2025)
### Changes
* Logging is improved.


## Version 2025.04.09.648  (9 April, 2025)
### Features
* Equities/balances tab is added to Risk management.
* Now it is possible to set a list of takers for each rule in Risk profiles => Rules.

## Version 2025.04.04.774 (4 April, 2025)
### Features
* The first version of Risk management tab is added.
### Changes
* Maker ID is added to the Makers table.

## Version 2025.04.03.785 (3 April, 2025)
### Changes
* Logs representation (in GUI) is improved.

## Version 2025.04.02.540 (2 April, 2025)
### Changes
* OneZero taker implementation is improved.
* Minor GUI bug (unknown GUI error when stopping the taker) is fixed.

## Version 2025.04.01.691 (1 April, 2025)
### Features
* "Limit as market" option is added to Risk profiles rules.
* "Volume percentage" option is added to Risk profiles rules.
### Changes
* "Import BP" function is improved (now even if hub symbols are added, the import function still will add the rest settings).

## Version 2025.03.28.530 (28 March, 2025)
### Changes
* The inner mechanism of order ID generation is improved to avoid ID duplication issues.


## Version 2025.03.27.618 (27 March, 2025)
### Changes
* In some cases it was impossible to edit NOP symbols values. This bug is fixed.

## Version 2025.03.25.869 (25 March, 2025)
### Changes
* Minor GUI changes (fixed the behavior of stuck columns).
* Log files improvement: taker name is used instead of taker ID in log files.
* Bucket volume calculation bug is fixed.
* The GUI bug of incorrect execution time for cancelled orders is fixed.
* Code refactoring (the handling of disabled makers/takers is improved).
* Risk profiles: makers tab GUI improvements.

## Version 2025.03.24.627 (24 March, 2025)
### Features
* Unifeeder maker connection is added (quotes only).
* Unifeeder taker connection is added (quotes only).
* Added some tooltips (with the hints) to Risk profile rules.

## Version 2025.03.19.687 (19 March, 2025)
### Changes
* Risk profiles rules table is rebuilt: it is made as a separate page instead of popup, some minor fixes are made.

## Version 2025.03.18.891 (18 March, 2025)
### Changes
* Improved the logic of building execution reports to pass them to takers.


## Version 2025.03.14.849 (14 March, 2025)
### Features
* Now it is possible to specify the part of order that must be confirmed on each maker in the list of rules (Risk profiles).


## Version 2025.03.12.472 (12 March, 2025)
### Changes
* FIX routing is improved.

## Version 2025.03.11.521 (11 March, 2025)
### Changes
* Minor logging optimizations.
* Minor GUI optimizations.

## Version 2025.03.10.373 (10 March, 2025)
### Changes
* The bug of incorrect password field (Users tab) representation is fixed.
* The validation of password expiration field (Users tab) is improved.
* USD currency is used to define and calculate NOP limits for symbols instead symbol currency.

## Version 2025.03.07.765 (7 March, 2025)
### Features
* TIF conversion tab is added to makers settings. Now it is possible to convert takers's orders TIF on makers side.

## Version 2025.03.06.428 (6 March, 2025)
### Changes
* The bug of incorrect slippage representation in orders/deals tables is fixed.
* Minor GUI improvements.
* "Import BP" function is improved (commissions and margin rates are added).
### Features
* Now it is possible to liquidate the position of maegin account with a single click.


## Version 2025.03.04.514 (4 March, 2025)
### Changes
* Logging the data is improved.
* "Allow all" makers checkbox bug is fixed.
* Incorrect symbols representation in margin account GUI is fixed.


## Version 2025.02.28.721 (28 February, 2025)
### Features
* Now it is possible to set the list of makers in Risk profiles (rules) that will be used for order confirmation.

## Version 2025.02.27.759 (27 February, 2025)
### Changes
* Price channels titles are fixed now when scrolling the page horizontally.

## Version 2025.02.26.652 (26 February, 2025)
### Changes
* The bug of risk profile rules were not applied (filetered by External login field) is fixed.
* FIX routing information are added to log files.

## Version 2025.02.24.916 (24 February, 2025)
### Features
* Now it is possible to apply risk profiles by External group name.
* Confirmation popup to price channels table is added.

## Version 2025.02.19.649 (19 February, 2025)
### Changes
* Logging is improved - minor logging bugs are fixed.

## Version 2025.2.17.636 (17 February, 2025)
### Changes
* It is possible to create several channel symbols (price channels) based on the same hub symbol;
* GUI optimization: speed up for Deals tab.

## Version 2025.02.13.693 (13 February, 2025)
### Changes
* Minor GUI visual fixes.
* "Import BP" function is added (allows to import symbols settings for some special setups).

## Version 2025.02.07.685 (7 February, 2025)
### Changes
* Extended logging for FIX messages in WebGUI.

## Version 2025.02.06.800 (6 February, 2025)
### Changes
* FXCubic Maker: additional routing rules have been added (ClOrdLinkID, Text);
* Removed the expiration time on A book quotes;
* Symbol relations tab has been removed;
* FOK option has been removed from FXCubic maker;
* Now it's possible to set makers list separately for each symbol.

## Version 2025.02.06.696 (6 February, 2025)
### Changes
* Fixed some buttons positioning.

## Version 2025.02.04.620 (4 February, 2025)
### Changes
* Added additional data for FX Cubic maker connection;
* Quote session unsubscribes in case maker's symbol is changed/removed.

## Version 2025.01.31.818 (31 January, 2025)
### Changes
* Added option for OneZero taker to receive and fill tag from external data.

## Version 2025.01.28.995 (28 January, 2025)
### Changes
* Added option to get account ID from FIX tag = 1 of 35=D FIX message and then put to External logic;
* Validation popup has been removed on leaving the market watch page;
* Minor visual changes.

## Version 2025.01.28.603 (28 January, 2025)
### Changes
* Volume factor parameter is called the same in all tables.
* Minor GUI changes.

## Version 2025.01.24.648 (24 January, 2025)
### Changes
* The inner logic of building web GUI tables is improved.
* FXCubic maker has been added;

## Version 2025.01.21.703 (21 January, 2025)
### Changes
* The bug of incorrect makers list displaying in price channels settings is fixed.

## Version 2025.01.17.439 (17 January, 2025)
### Changes
* The bug of incorrect hub symbols import/export is fixed.
* The bug of incorrect quote number per minute is fixed.

## Version 2025.01.15.690 (15 January, 2025)
### Changes
* Some more flexibility is added to price channel configuration.

## Version 2025.01.10.648 (10 January, 2025)
### Changes
* MatchTrade maker connection is updated according to new documentation.
* Inner optimizations.

## Version 2025.1.9.882 (9 January, 2025)
### Changes
* The hub is migrated to .NET 9.0


## Version 2024.12.27.769 (27 December, 2024)
### Changes
* 4 charts are added to Overview tab.

## Version 2024.12.24.888 (24 December, 2024)
### Changes
* Some cosmetic GUI changes are added and bug fixed.
* The GUI bug is fixed: in some cases the GUI did not displayed the current maker list.

## Version v2024.12.20.271 (20 December, 2024)
### Features
* Added bid and ask maker columns for market watch;
* Position adjustment for margin accounts is improved.

## Version 2024.12.17.665 (17 December, 2024)
### Features
* Price representation is added to position adjustment window (Accounts tab, account position).
* FIX connection to Brokeree is added.
* The bug when it is not possible to create price channel was fixed.
* Several inner performance improvement.

## Version 2024.12.13.418 (13 December, 2024)
### Changes
* Inner performance optimizations.

## Version 2024.12.12.712 (12 December, 2024)
### Changes
* Additional hub symbols export options were added (export in price channel format and maker symbols format).
* Fixed the bug of price symbol duplication.
* Several inner performance improvement.

## Version 2024.11.27.791 (27 November, 2024)
### Changes
* Internal improvements have been made to improve performance and optimization.
### Features
* NOP limit profiles logic is added. 

## Version 2024.11.20.688 (20 November, 2024)
### Changes
* Added hub symbol name to "Symbols mapping" tab (takers).
* Makers list configuration of the price channel is improved.

## Version 2024.11.13.857 (13 November, 2024)
### Features
* Now it is possible to enable/disable symbol processing inside of the price channel.

## Version 2024.11.08.842 (8 November, 2024)
### Changes
* Some notifications that are not actual are removed.

## Version 2024.11.06.657 (6 November, 2024)
### Changes
* Minor table filtration changes.

## Version 2024.11.04.1051 (4 November, 2024)
### Changes
* Db handling on the start is optimized (important if the database size is really big).
* TSV file wrong import notification text is fixed. 
### Features
* Now it is possible to set the list of makers that will be providing prices and fillig orders for the chosen priec channel.

## Version 2024.10.28.604 (28 October, 2024)
### Changes
* Makers priority (hub symbols) bug is fixed.
* Several minor inner errors are fxied.
* Minor GUI bug fixes.
### Features
* It is possible now to import log files from the GUI for further investigations.

## Version 2024.10.24.61 (24 October, 2024)
### Changes
* Huge speed up of the hub starting process.
* Inner code structure is optimized and safety improved (maker/taker connections).

## Version 2024.10.21.721 (21 October, 2024)
### Changes
* Representation of risk profiles tab is improved.
* Minor data representation improvements.

## Version 2024.10.17.490 (17 October, 2024)
### Changes
* Stick ID of orders, positions, deals, positions history, account history tables when scrolling horizontally.
* Now it is possible to customize (show/hide the columns) tables: orders, deals, positions, positions history, accounts history, equity reports.

## Version 2024.10.15.262 (15 October, 2024)
### Changes
* BUG fixed: there were some cases the taker order ID is duplicated.
* Symbols mapping table is added to Takers tab.
* Added new maker: Centroid.

## Version 2024.10.14.897 (14 October, 2024)
### Changes
* Some minor data representation fixes.

## Version 2024.10.10.992 (10 October, 2024)
### Changes
* BUG fixed: the filteres was not applied to exported data (Export/Import to csv).
* BUG fixed: the exported data contained exponential values.
* BUG fixed: NOP limit was defined incorrectly because of wrong price for conversion was taken.
* BUG fixed: sometimes the position was not marked as closed in database and remained open.
* NOP logic is improved and placeholders are added to NOP limits popup.
* The filters is not prefilled by current date anymore.
* Some typos are fixed.
* Fixed the IDs or orders/deals/positions: somewhere they were stored without the identifiers (O, D, P).

## Version 2024.10.04.419 (4 October, 2024)
### Changes
* Major FIX price processing optimization - the maximum number of price processed per second increased on ~30%.

## Version 2024.10.03.526 (3 October, 2024)
### Changes
* Text of "Send order" popup (to maker) is changed.
* The bug of negative eecution time is fixed.
* Several typos in GUI are fixed.

## Version 2024.10.02.459 (2 October, 2024)
### Changes
* The names and buttons of Takers/Accounts are stuck on the left side - the y don't move when scrolling page to the right.

## Version 2024.09.30.798 (30 September, 2024)
### Changes
* Import/export bugs of hub symbols are fixed.
### Features
* Now it is possible to customize the columns of Takers and Accounts tabs (choose what columns must be displayed).

## Version 2024.9.28.718 (28 September, 2024)
### Changes
* Takers/Accounts search field bug is fixed.

## Version 2024.09.27.497 (27 September, 2024)
### Changes
* Added the oportunity to search Takers and Accounts on their pages.

## Version 2024.09.26.702 (26 September, 2024)
### Changes
* The bug of incorrect price displaying (maker => send order) is fixed.

## Version 2024.09.20.459 (20 September, 2024)
### Changes
* 'Estimated total' in Databases > Deals has been renamed to 'Total Deals'.
* Execution issues on the Binance Futures maker have been resolved.
* Fix messages bug has been resolved for PXM-related issues.
* IgnorePartialFillsExceptGTC parameter has been removed for PXM taker.

## Version 2024.09.18.303 (18 September, 2024)
### Changes
* Events tab is added.

## Version 2024.09.17.663 (17 September, 2024)
### Changes
* Filters searching has been sped up.

## Version 2024.09.13.756 (13 September, 2024)
### Features
* Added chart to Market watch.
* Added 2 new metrics (and the corresponding charts to Grafana): the total profit in USD from markups and the total trading volumes by core symbols converted to USD.
* Added 'Symbols relations' tab to 'Settings'.
* Added filter to 'Price channels'.
* Discrepancy in 'Exposure' window is now highlighted.
### Changes
* 'Reports' tab is removed from the main menu.
* The bug with priority list checking has been fixed.
* Minor bugs have been fixed.
* Default volume value has been hidden and hardcoded.

## Version 2024.08.28.718 (28 August, 2024)
### Changes
* Fixed issue linked to execution reports sending.

## Version 2024.08.26.817 (26 August, 2024)
### Changes
* ExternalTradingAccountId FIX routing option is added.

## Version 2024.08.15.684 (15 August, 2024)
### Changes
* It is possible to send MT trading account ID to PrimeXM makers.
* Total USD volume of the deals is calculated by the hub and represented on Deals tab.
* Partial execution bug is fixed.
* Active orders table: timeout of data update is set to 10 minutes instead of 10 seconds. 

## Version 2024.08.08.688 (8 August, 2024)
### Features
* Overview page has been added with Grafana charts compatibility;
### Changes
* The bug of GUI log files were cut is fixed.

## Version 2024.08.05.648 (5 August, 2024)
### Changes
* Database optimization - the orders that are splitted between A-book and B-book now can be processed a bit faster.

## Version 2024.07.24.761 (24 July, 2024)
### Features
* It is possible to write the data to db asynchronously.

## Version 2024.07.16.751 (16 July, 2024)
### Changes
* The view of maker priority list (hub symbols) is made as checkbox list.

## Version 2024.07.15.1049 (15 July, 2024)
### Changes
* GUI bug is fixed: unhandled exception when trying to edit maker/taker.
* OKX maker connection errors are fixed.

## Version 2024.07.03.652 (7 July, 2024)
### Changes
* Added more informatin about execution time to log files.
* Incorrect name of imported risk profile csv file is fixed.
* Added a possibility to switch logging modes on the fly withour restrating taker or maker connections.


## Version 2024.06.28.692 (28 June, 2024)
### Changes
* It is not poossible to set the default ports for takers (appsettings.json) to speed up taker creation.

## Version 2024.06.24.426 (24 June, 2024)
### Changes
* Comment field is added to risk profile rules.
* Instruments.csv file is not needed no more for PrimeXM and Integral takers.
* Fixed the bug when the orders were rejected because of quotes timed out.
* Minor GUI bugs are fixed.
* Log files are extended: now the stuck orders are added to log files for investigations.
* The bucket logic is rebuild: the bucket volume will not be fully sent to LP if the limit is exceeded.

## Version 1.343 (24 May, 2024)
### Changes
* Several performance features was implemented. For some cases there was unexpected latency, that was fixed.

## Version 1.332 - 1.339 (27 April - 17 May, 2024)
### Features
* Adding log displaying to rder and deal details windows.
* Delay logic is improved - the operational delay now is a part of overall delay.
### Changes
* Massive code refactoring.

## Version 1.331 (24 April, 2024)
### Changes
* Manual rejection bug is fixed.
* Partial execution (A-book + B-book) bugs are fixed.
* Position adjustment logic is fixed.
* Total PnL and Closed PnL columns are added to margin accounts tab.

## Version 1.328 (22 April, 2024)
### Changes
* The bug of incorrect margin account volume displaying is fixed.
* Hub symbol description column is added.
* Exposure calculation for B-book part is improved.
* Read only users: order details displaying bug is fixed.

## Version 1.326 (17 April, 2024)
### Features
* Now it is possible to assign B-book account from margin account menu.
### Changes
* The additional settings verifications are added.
* Hub symbols search is improved.
* Risk profile creation bug is fixed.
* Order details bug is fixed.

## Version 1.317 - 1.323 (1 April, 2024)
### Changes
* "Searching" bug is fixed.
* Minor GUI changes.
* Change the logic of displaing partially filled orders.
* Bucket logic is improved.
### Features
* The volume filter is added to Risk Profile rules.

## Version 1.316 (27 March, 2024)
### Changes
* Minor GUI changes.
### Features
* It is possible to set partial B-book execution.
* B-book accounts part is added.

## Version 1.311 (12 March, 2024)
### Changes
* Minor GUI changes.
* Additional validation for hub symbols creation is added.
* Partial execution logic is improved (dropcopy FIX session).

## Version 1.308 (9 March, 2024)
### Changes
* Risk profile rules tab is optimized.
* Now it is possible to sort takers by name, type and state.
* Incorrect displaying of maker positions is fixed.

## Version 1.307 (5 March, 2024)
### Changes
* Inner SQL requests are optimized.

## Version 1.306 (3 March, 2024)
### Changes
* Minor GUI changes.
### Features
* Now it is possible to apply slippage to orders, executed in B-book.
  

## Version 1.305 (1 March, 2024)
### Changes
* FIX engine logic is optimized.

## Version 1.304 (26 February, 2024)
### Changes
* Minor GUI changes.
* Bug of incorrect takers displaying.

## Version 1.300 - 1.303 (12 February, 2024)
### Changes
* Routing tab bugs are fixed.
* Minor GUI improvements.
* Text of several errors is improved.
* Margin accounts "empty list" bug is fixed.

## Version 1.299 (9 February, 2024)
### Changes
* Manager (read only) rights bugs are fixed (the read only manager could change configuration before).
* Minor GUI improvements.
### Features
* Now it is possible to assign price channel and margin account from taker's settings.

## Version 1.298 (5 February, 2024)
### Changes
* Minor GUI improvements.
### Features
* Main menu is frozen when scrolling the page.
* Routing tab (by margin account) is added for makers (before it must be possible to set routing only with ternary operator).

## Version 1.293 (24 January, 2024)
### Changes
* Auto-logout mechanism is removed (the user had been logged out by the hub every 10 minutes before).
* Removed the opportunity to set partial B-book for margin accounts.
* Minor GUI improvements.
* Symbols filtration is added to market watch.

## Version 1.289 - 1.292 (22 January, 2024)
### Changes
* API keys generation mechanism for users are addeed.
* Title is added to the GUI.
* Position deletion mechanism is improved.
* Added an oportunity to choose the price when placing limit order on maker side.

## Version 1.288 (14 January, 2024)
### Changes
* OKX trading logic is added.

## Version 1.287 (13 January, 2024)
### Changes
* The hub is migrated to .net framework version 8.

## Version 1.286 (12 January, 2024)
### Changes
* Added routing by tag=1 for Integral taker.
* Spread value is added to market watch of all users of the hub.
* Minor inner logic bugs are fixed.

## Version 1.281 - 1.285 (11 January, 2024)
### Changes
* Price channel bugs are fixed (it was not possible to create/change price channel in some cases).
* Integral taker bugs are fixed.
### Features
* Dropcopy session is added for Integal taker.

## Version 1.279 - 1.280 (23 December, 2023)
### Changes
* Configuration templates' errors are fixed.
* Reports tab is added.
* "FIX sessions can't be downloaded" bug is fixed.
* "Channel" column in Market watch of margin account is removed.
### Features
* OKX maker is added: pricing part.
* Spread value is added to the market depth for each layer of depth.


## Version 1.278 (20 December, 2023)
### Changes
* Binance maker's issues are fixed.
* Some minor bugs are fixed.
### Features
* Now it is possible to download taker's FIX credentials as .ini file after they are created.

## Version 1.277 (12 December, 2023)
### Changes
* Minor inner logic bugs are fixed.
* Minor GUI bugs are fixed.

## Version 1.273 - 1.276 (8 December - 11 December, 2023)
### Changes
* Minor bugs are fixed.
* "Refresh" buttons are removed from all pages.
* Some minor design changes.
* Fields values validation mechanisms are improved.

## Version 1.272 (7 December, 2023)
### Changes
* Minor GUI changes.
* Input fields validation logic fields is improved.
* Syncfusion migration is complete.
* Starting of maker/taker is improved.
* GUI bugs are fixed.

## Version 1.271 (4 December, 2023)
### Changes
* Hints when hovering the buttons are removed.
* Minor GUI changes.

## Version 1.270 (3 December, 2023)
### Changes
* Minor GUI changes.
* TSV import/export logic is improved: now import or export is amde as atomic operation.

## Version 1.269 (29 November, 2023)
### Changes
* Password expiration bug (Users tab) is fixed.
* Error is fixed during hub stopping process.

## Version 1.246 - 1.268 (12 November - 27 November, 2023)
### Features
* Password settings are added to Users tab.
* Market watch is added for Margin account (read only) role.
* Margin account (read only) role is added.
* Now it is poossible to change the style of hub's GUI by changing inner css file (css file is not hardcoded anymore).
* BookHandlingExpirationTimeInMs parameter is added.
### Changes
* Trade details page is migrated to Syncfusion frontend framework.
* Trade details page is migrated to Syncfusion frontend framework.
* Position Reports table is migrated to Syncfusion frontend framework.
* Users table is migrated to Syncfusion frontend framework.
* The performance of the hub was improved.
* Takers working logic was improved (now each taker's quotes are processed separately from other taker and does not affect theit quote processing logic).
* FIX subscription logic was imporved (now there is no issue when hub tries to subscribe to huge amount of symbols at the same time).
* "Slow taker" is fixed (now slow taker does not affect other takers).
* Code optimization.
* Start/stop taker process is speeded up.
* Unnecessary metrics are removed.
* FIX default session is added back to taker's FIX connection settings.

## Version 1.245 (11 November, 2023)
### Changes
* Margin account positions table is migrated to Syncfusion frontend framework.
* Margin accounts table is migrated to Syncfusion frontend framework.

## Version 1.244 (9 November, 2023)
### Changes
* FIX unsubscription logic is improved: now the hub does not check the existence of the symbol before unsubscription.

## Version 1.242 (6 November, 2023)
### Changes
* Incorrect FIX taker templates are fixed.

## Version 1.241 (31 October, 2023)
### Changes
* Risk Profiles table is migrated to Syncfusion frontend framework.
* Page loading speed is improved.

## Version 1.239 (25 October, 2023)
### Changes
* Makers table is migrated to Syncfusion frontend framework.
* Minor GUI changes.
* Monitoring system bug is fixed.
* Bug fixed: it was not possible to send the order from taker side (hub's GUI).
* Logon page validation logic is improved.

## Version 1.237 (18 October, 2023)
### Changes
* Takers table is migrated to Syncfusion frontend framework.
* Maker/Taker templates are hardcoded and removed from hub's Contents folder.
* Minor GUI changes.
* Multiple Integral taker bug fixes.

## Version 1.235 - 1.236 (6 October, 2023)
### Features
* Integral taker is implemented.
### Changes
* Auto logout issue is fixed (now the hub log out the user if it is logged in but not active for some time).
* Minor GUI changes.
* USD exposure calcualtion bug is fixed.

## Version 1.234 (4 October, 2023)
### Changes
* New type of rejects are added (rejects by hub core).
* Incremental price update logic is improved.

## Version 1.233 (3 October, 2023)
### Features
* USD exposure table is added to Exposure tab.
### Changes
* XTRD resubscription logic is implemented.
* Taker/Maker FIX settings template is changed (default section is removed).
* Minor GUI fixes

## Version 1.232 (1 October, 2023)
### Changes
* Some minor changes for exposures table are added.
* LmaxMTF and LmaxMTFWesternPips are merged to one maker type.

## Version 1.231 (28 September, 2023)
### Changes
* Price Channel tab is migrated to Syncfusion frontend framework.
* Market watch optimization.

## Version 1.230 (26 September, 2023)
### Changes
* Bug fixed: prices haven't shown when trying to send order from the hub side to maker.

## Version 1.228 (19 September, 2023)
### Changes
* Incremental market data refresh bug is fixed.
* Exposure calculation bug is fixed.

## Version 1.227 (18 September, 2023)
### Changes
* Exposure table loading bug is fixed.

## Version 1.226 (17 September, 2023)
### Changes
* FIX sessions disconnection mechansm is improved.
* All checks when creating user is removed.

## Version 1.225 (14 September, 2023)
### Features
* Currencies are added to Exposure tab.
* Inner order generator (test taker) is improved.
### Changes
* Changing administrator name bug is fixed.
* Incoming quote handling is improved.

## Version 1.224 (11 September, 2023)
### Features
* Currencies are added to Exposure tab.
### Changes
* Changed double dropdown menu bug in the GUI.

## Version 1.223 (10 September, 2023)
### Changes
* Margin account representation in Exposure table is changed (now takers are groupped by margin account).
* Lmax maker is renamed to LmaxMTF.

## Version 1.222 (8 September, 2023)
### Features
* SolidFX maker is added.
* Representation of market depth is changed.
### Changes
* Minor GUI changes.
* Changed default number of book layers to subscribe for makers to 5.

## Version 1.220 - 1.221 (2 September, 2023)
### Features
* Simple aggregation logic failover is changed (now it failover works for each symbol instead of the whole maker).
* Advanced aggregation logic failover is changed (now it failover works for each symbol instead of the whole maker).
### Changes
* Fixed Prometheus integration bug (older versions were incompatible with new config file). 

## Version 1.218 - 1.219 (29 August, 2023)
### Features
* Tab "Exposure", table "Symbols" is added.
* "Execution time 50%" column is added to home page.
* "Execution time 90%" column is added to home page.
* Vertical and horizontal scrolls are removed from tables (and only page scrolls are left).
* "Market depth" of Symbols table is completely rebuilt.
* "Type" column is added to main page table to show FIX API each maker/taker uses.
### Changes
* Inner methods refactoring.

## Version 1.217 (25 August, 2023)
### Features
* "Symbol subscription" column is added to home page.
* "Exposure" tab is added.
### Changes
* Minor GUI changes.
* cTrader FIX acceptor is improved.

## Version 1.216 (19 August, 2023)
### Features
* "OrdersPerMinute" column is added to home page table.
* "QuotesPerMinute" column is added to home page table.
### Changes
* Inner quote processing is improved (on taker's side).
* PrimeXM acceptor is improved.

## Version 1.213 - 1.215 (12 August, 2023)
### Changes
* All the tables are migrated to Syncfusion framework.
* Background color is changed to white.
* Gradients are removed from all the pages.
* Buttons form is changed to rectangle.
* Font color is changed to #5C0658.
* Button text is changed to white.
* Button color is changed to #5C0658.
* Link color is changed to #1B6AC9.
* Tables color is changed to white.
* Fonts are changed to Roboto Regular.
* Title font size is changed to 18px.
* User authentication bug is fixed.
* Prometheus connection bugs are fixed.
* Removed old table form home screen.
* Home page data representation is remade.

## Version 1.212 (12 August, 2023)
### Features
* Prometheus client is added.

### Changes
* Improved incremental price update workflow.
* Depth of market creation mechanism is improved.
* Bucket logic is improved (the hub does not send bucket order if there is no pricing).

## Version 1.211 (8 August, 2023)
### Changes
* Execution delays bug is fixed (inner loggin mechanism is improved).
* Removed extra tags from 35=X FIX messages (MdEntrySize).
## Version 1.210 (24 July, 2023)
### Features
* REST API server is added.
* REST commands to enable/disable takers are added.
* "SubscribeToIncrementalUpdates" is added to quote providers (to subscribe on incremental quote refresh if available).
### Changes
* GUI working logic optimization - additional GUI libraries were added.
* Firefox GUI representation is improved.
* Market watch is improved with updated frontend libraries.
* GUI minor improvemnets.
* Quote processing bug is fixed.
* Quote subscription (FIX) bug is fixed.

* ## Version 1.209 (10 July, 2023)
### Changes
* Minor redesign of the GUI.
* "Overview" menu item to main menu is added.
* "Market watch" is added to "Overview" as menu item.
* "Home" tab is moved to "Overview".
* "Market watch" inner table is added.
## Version 1.207 (5 July, 2023)
### Changes
* Bug fixed: under some conditions there was an exception when adding new hub symbol.

## Version 1.206 (7 July, 2023)
### Features
* Synthetic symbols generation is added (for this version there are only quotes).
* The execution time in milliseconds is added to margin account report.
### Changes
* Inner book generation is optimized.
* BidPriceAtConfirmation data was added for margin account report.
* AskPriceAtConfirmation data was added for margin account report.
* Bug fixed: db disconnection process is handled correct starting this version.

## **Version 1.204-1.205 (29 June, 2023)**
### Features
* Added display of password complexity when creating a new user.
* TakerRequestedPrice column added to margin account report 
### Changes 
* Fixed a bug due to which the tab with the order table did not open.
* Internal changes with books aggregation.
* Minor displaying bugs fixed.

## **Version 1.203 (15 June, 2023)**
### Features
* Added filtration for synthetic symbols.
* Added T4B acceptor
* Added “Execution time” column in orders table.
* Added “Order price slippage” column in orders table.

## **Version 1.202 (9 June, 2023)**
### Features
* Added working logic for synthetic symbols.
* Added a new index (order_time_stamp_idx) to the internal_order table. (internal change in database)
### Changes 
* Minor displaying bugs fixed.
* Fixed loading error on homepage.
* MakerExecutedPrice, TakerRequestedPrice, MakerTradeId, TradeDate, MakerSlippage columns were removed from margin account report

## **Version 1.197-1.201 (1 June, 2023)**
### Features
* Added report to margin account in web GUI.
* Added logic of margin account report generation.
* Added fields for synthetic symbols in web GUI.
* XTRD Maker was added.
### Changes 
* Fixed error with filling MakerExecutedPrice, MakerExecutionDurationMs, HubExecutionDurationMs, MakerTradeId,MakerSlippage columns in margin account report.
* Trading session support has been removed from XTRD maker.

## **Version 1.195-1.196 (10 May, 2023)**
### Features
* Added Lmax Taker.
* Added ProviderBookQueueCapacity parameter.
* Added new metrics method to display quotes that were not cached
### Changes 
* Fixed order cancel message in OZ maker,  if during timeout order not executed hub send 35=F (order cancel) multiply times.
* Fixed stuck order message in PrimeXM maker,  if during timeout order not executed hub send 35=H (OrderStatusRequest) multiply times.
* Made code refactoring relating to providers books.

## **Version 1.194 (19 Apr, 2023)**
### Features
* Added Exposure data to margin account GUI.
### Changes 
* Fixed pages loading.
* Fixed GUI loading indicator.
* Fixed text style on Home page.
* Fixed head of table color on Home page.
* Fixed quotes stop on Hub Symbols tab.
* Fixed session order bug in Fortex maker.
* Home tab moved to Syncfusion library.
* Fixed bug, on two console logger.

## **Version 1.192 (14 Apr, 2023)**
### Changes 
* MarketGTCTimeOutMs - logic changed, if during timeout order not executed hub send 35=F (order cancel) multiply times.
* Added reject order if unknown status from Fortex maker.
* Added notification about discrepancy between Hub maker and LP after order cancellation.
* Added status requests for stuck orders to Prime XM maker.


## **Version 1.191 (10 Apr, 2023)**
### Features
* Added DisableFixQuotesLogging=Y/N to takers.
### Changes 
* Code refactoring.
* Changed digits number in 35=8 message of order was rejected by Exposure Limit logic.
* Added "MinimumLogLevel": "Information" as default setting.
* Fix logs moved from Debug level to Information level.
* Application/Request logs reworked.
* Fixed bug, Exposure Limit logic not working.
* Remover Invalid state in 37 tag when order status unknown.
* Fixed bug, hub feed to csv only 35=i messages on PXM taker.

## **Version 1.189 (24 Mar, 2023)**
### Features
* Added SaveQuotesToLog=Y/N to takers.
* Added Exposure limit logic:
* Exposure column to margin accounts table.
* Exposure Limit column to margin accounts table.
* Exposure Limit to margin account settings.
### Changes 
* Binance makers no quotes bug fixed.
* Fixed incorrect makers/takers connection state.
* Added config default filling if object is deleted.
* Added nullable references (code refactoring).

## **Version 1.188 (17 Mar, 2023)**
### Changes 
* Fixed bug, port occupancy when taker is disabled.
* Fixed bug, of test request sending error while connecting taker/maker.
* Fixed exception error while adding edits to margin account with no taker. 
* Inner changes, code refactoring.

## **Version 1.187 (10 Mar, 2023)**
### Changes 
* cTrader taker: made the MDUpdateType (265) tag optional in the MarketDataRequest (35=V) message.
* Added simple path validation to ConfigureMetricServer method.
* Added possibility to check the product version for Linux HUB.
* Added null check to QuickFix engine.


## **Version 1.186 (9 Mar, 2023)**
### Features
* Allowed both, IP and host name format in SOCKET_ACCEPT_HOST.
### Changes 
* Fixed sequence number resetting on maker reconnection.
* Fixed returning correct code if service crush.
* Fixed bug with non-existent subscriptions in the FIX Provider.
* Removed MT4ManagerAPI and MT4ToolBase project references from hub.
* Fixed the InstrumentsFile option default value in provider/consumer configs.

## **Version 1.185 (22 Feb, 2023)**
### Features
* Added https support.
### Changes 
* Changed WebServiceToolsLegacy to WebServiceTools.
* Changed the consumer/provider startup logic.
* Changed reset sequence number reset logic.
* Fixed HUB GUI start logic.
* Increased storage memory size (10K).
* Added session checking if IResponder is disconnected.
* Fixed rejection of incorrect messages to hub.

## **Version 1.182 (10 Feb, 2023)**
### Features
* Added ability to enter negative markup values in points, price channel.

## **Version 1.181 (8 Feb, 2023)**
### Changes 
* Added name of symbol to subscription reject message (35=Y).
* Removed default values for Timestamps in Hub.Interfaces.
* Added filling 150=I, order status.
* Added partially filled order in fix messages.

## **Version 1.180 (20 Jan, 2023)**
### Features
* Added TakeprofitCentroid acceptor.
### Changes 
* Added 35=8 message with order status.
* Added 35=8 message with leavesQty (tag 151).
* Fixed OnBehalfOfCompID duplication OZ connector.

## **Version 1.179 (14 Jan, 2023)**
### Features
* Added filters to Hub Symbols tab.
* Added “Delete” button to Hub Symbols tab.
### Changes 
* Fixed 35=W and 35=i calculation on PrimeXM acceptor.
* Fixed filter checks in core symbol.
* Fixed displaying commission per million risk profile.
* Fixed ExecType in report in TPT Taker.
* Reworked "Cancel all" and "Reject all" buttons, Active Orders.
* Hub updated to .Net 7.0.
* Hub refactored to .Net 7.0.
* QuickFix actualized.
* QuickFix refactored.
* Fixed maker creation freeze.

## **Version 1.177 (14 Dec, 2022)**
### Features
* Added Cancel and Reject buttons to Active orders tab.
### Changes 
* Changed style of all hub buttons.
* Added trade websocket to Binance Futures/Spot.
* Fixed inner logic of quote steam rules at provider.

## **Version 1.176 (12 Dec, 2022)**
### Changes 
* Fixed bug with modified collection.
* Fixed AggregateBooks method.
* Added support for sending custom tag 1 (Account) in OZ Maker.
* Added cancel order support to TPT fix maker.
* Fixed methods in OrderHelpers and BookHelpers to use mutable collections.

## **Version 1.175 (08 Dec, 2022)**
### Features
* Added vertical scrolling to book page core symbols.
### Changes 
* Added soft loading animation to Core Symbols page.
* Added soft loading animation to Editing Symbols page.
* Added soft loading animation to Creating Maker page.
* Added soft loading animation to Creating Taker page.
* Added soft loading animation to Creating/Editing page.
* Added soft loading animation to Price Channel page.
* Added soft loading animation to Risk Profile page.
* Added soft loading animation to Provider Rules page.
* Added soft loading animation to Core Symbols page.
* Added soft loading animation to Core Symbols page.
* Added displaying b-book values at orders tree.
* Fixed console mode stopping.
* Added prompt to price channels rules.
* Fixed order cancellation to Fortex acceptor.
* Added order cancellation to PrimeXM acceptor.
* Added fatal error if database have no free connections.
* Fixed bug TSV orders reports does not apply maker filter.


## **Version 1.173 (30 Nov, 2022)**
### Changes
* Changed format of volume step at backup TSV files.
* Changed name of VolumeMultiplier to VolumeFactor at backup TSV.
* Fixed bug: Exception while hub stopping at console run.
* Added Ignore status requests on hub stopping.
* Enforced session status check.
* Added soft page loading animation at hub startup.
* Added soft page loading animation while TSV, CSV import process.
* Replaced edit button at users tab.
* Fixed takers displaying at margin accounts tab.
* Fixed margin account displaying at risk profile tab.
* Changed rounding mechanism at margin accounts table.
* Added page cache clearing.

## **Version 1.171 (21 Nov, 2022)**
### Features
* Added SaveQuotesToLog, DisableQuotesLogging to Kraken connector.
### Changes
* Fixed a bug when subscribing to Binance Futures symbols.
* Removed additional Binance Futures subscription check before connecting wss.
* Added SeqNum clearing in app cache.
* Fixed message text when hub acceptor cannot connect.
* Added 35=1 message to hub acceptor, sending every minute, response 35=0.
* Added 35=1 message to hub connector, sending every minute, response 35=0.
* Added database connect to ip address and port to hub logs.

## **Version 1.170 (28 Oct, 2022)**
### Features
* Added dropcopy session at takers settings.
* Added UseSecondaryClOrdID setting to PrimeXM Maker, can be Y or N. If Y, 526 tag will fill with name of the party who originates order.
* Added cTrader acceptor.
* Added ability to get TSV reports from Orders and Positions History tabs for margin account.
* Added protection against duplicate fix sessions.
### Changes
* PrimeXM acceptor 35=i message is fixed.
* Added 35=W message added to PrimeXM acceptor.
* Fixed bug, core symbols do not have auto update.
* Added autocorrection of TSV file while import.
* Fixed stream rules editing bug.
* Added only enabled taker/makers validation.
* Added fatal error at start if duplicated sessions obtained.

## **Version 1.168 (28 Sep, 2022)**
### Features
* Added ability to change between dev and client types of hub.
### Changes
* Added protection against SQL injections.
* Freeze all information columns at hub tables.
* Added links to hub tables.
* Added a HUB call of the ANALYZE DB function every Sunday.
* Added ping connection at Kraken maker.
* Added autofilling of SessionQualifier at B2C2 maker.
* Changed archive logs destination folder.
* Fixed bug: cannot add new taker.
* Add zero quotes ignoring.

## **Version 1.165 (13 Sep, 2022)**
### Changes
* Fixed bug of migration to the next version of the database.
* Code formatted and libraries updated.
* Removed restriction to use SessionQualifier with acceptor connection type.
* Added button freeze when applying marker settings.
* Added splitting Batch request into chunks.

## **Version 1.161 (29 Aug, 2022)**
### Changes
* The hub build for Linux is packaged in a single executable file.
* Changed the logic of tag 35=D when tag 115 is used.
* Fixed test crashes on the Linux.

## **Version 1.160 (27 Aug, 2022)**
### Features
* Your Bourse connector added to HUB Makers.
* Added a popup when a limit order is successfully placed in the GUI.
* Added BookUpdatePeriodMs parameter to Binance connectors.
* Added MaxStreamsPerConnection parameter to Binance connectors.
### Changes
* Fixed update of quotes in the cache.
* Removed internal order from deals request.
* Removed deals from orders query.
* The operation of the .Net Core library has been changed. Library files are no longer saved to the Temp folder (Windows System).
* Added database ANALYZE function to get statistics on HUB tables (starting with EOD).
* Added removing of data on detached takers' symbol prices from the cache and position_last_price table.
* Added conversion rate updating according to the position key (position_last_price table).
* Alpaca Maker book update optimized.
* Changed the hint text when an incorrect value is entered in the Default BBook Part (Risk Profile).
* Added updating position last price cache keys when updating quote streams.
* Optimized requests for EF orders and deals.
* When importing a TSV file with symbols, the Priority field is ignored.
* Fixed precision bug in compress tool.


## **Version 1.158 (19 Aug, 2022)**
### Features
* The number of decimal digits for margin and conversion rate values in the EOD report is limited.
Made a TPT HUB build running on Ubuntu Linux.
### Changes
* Added possibility to take conversion rates from positions in case of no quote on conversion symbols.
* The SELECT query to the database stops if the user closes the window with the query.

## **Version 1.157 (8 Aug, 2022)**
### Features
* Added CHF (Finalto) connector.
* Added B2C2 connector.
* Added the ability to set a rule per symbol without specifying a swap volume.
* Added a pop-up window when trying to put a price channel with the same symbol on one taker.
### Changes
* Fixed bug: incorrect license check at service start.
* Fixed reset of sequence number on the maker's trading session. If there were no changes in the maker settings, the sequence number is not reset. 
* A delay of 15 seconds is added when the hub stops, this time is given for the execution of orders.
* Fixed error: "Error on swap apply: Sequence contains no elements”.
* The license check is migrated from C++ to C#.
* Fixed order reject on maker connection problem.

## **Version 1.154 (28 Jul, 2022)**
### Features
* Added formatting of the value when entering trade quantities.
* Removed charging a commission on the maker's side when adjusting positions.
* Added display of a symbol in a popup window when an order is executed.
* Changed the name of the columns in the Rules menu, Risk Profile settings. 
### Changes
* Fixed bug: Incorrect display of volumes in the margin account window.
* Fixed conversion rate rounding in EOD report.

## **Version 1.153 (14 Jul, 2022)**
### Features
* ID’s ignores while import hub symbols via TSV file.
* Added IgnorePartialFillsExceptGTC=Y/N parameter, if Y (yes), PrimeXM taker have no partial repots.
* For Xenfin maker, ResetOnLogon parameter is Y (yes) on default.
### Changes
* Bug fixed: Incorrect time display.
* Bug fixed: Margin account wrong value withdrawal.
* Symbol name specified in symbol overrides log.

## **Version 1.152 (02 Jul, 2022)**
### Changes
* Changed the error text when Binance connectors are connected unsuccessfully.
* Fixed bug: Displaying a single position in EOD report.
* Fixed FATAL ERROR display on unsuccessful connection to database.
* Fixed bug: The BUY/SELL buttons are active without a price for the symbol.
* New table for storing prices and conversion rates from cache added to the database.
* Added checking of invalid positions.
* Fixed process of stopping invalid positions.
* Added local cache of prices for NET-positions.
* Fixed the calculation of Conversion Rate for NET-positions.
* Changed the InitProfitsProperties backend method (used to calculate the NET position profit).

## **Version 1.151 (21 Jun, 2022)**
### Features
Added Alpaca Markets live trading (Stock, Crypto).
### Changes
Added symbol subscription deviation if it is not in price channel.
Added a popup window in the case of a reject (as an example, the provider does not support the selected TIF), the main window in the case of a reject is not closed.

## **Version 1.150 (15 Jun, 2022)**
### Features
* Apply Changes button in risk profiles, rules inactive if no changes added.
* Buttons “Delete” and “Edit” are deleted from positions tab.
### Changes
* Added symbol check before subscribe Kraken connector.
* Added rate limits to Alpaca connector.
* Changed format of error while connection (maker/taker) forcible interrupted.
* Alpaca Markets Paper API updated.
* Added new logic of net-position calculating.
* Added symbol check before subscribe Alpaca connector.
* Alpaca subscription changed, no requests if market are closed.
* Changed type of HTTP requests at Kraken, OkCoin and Alpaca connectors.
* Binance rate limit changed. 

## **Version 1.148 (03 Jun, 2022)**
### Features
* Added Orders tab for Margin Account Manager.
* Added Account History tab for Margin Account Manager.
* Added Deals tab for Margin Account Manager.
* Added Position History tab for Margin Account Manager.
* Added Positions tab for Margin Account Manager.
* Added order details for Margin Account Manager.
### Changes
* Added subscription to symbols without restarting Binance SPOT connector.
* Fixed a bug, an error when making a comment in the main administrator's record.
* Changed the address of the monitoring system for processing hub logs.
* Fixed a bug where it was impossible to use the "/" sign in the name of the risk profile rule.
* Fixed bug, the lack of visibility of the chains of execution of the order for the admin.
* Changed logging when configuring maker symbols and price channels.
* Added detailed message logging at Hub Reject level.
* Changed how the cache memory in the hub works, the quotes of non-priority makers are stored so that outdated quotes do not come when switching.
* Fixed bug when setting invalid SocketAcceptHost in taker settings.

## **Version 1.146 (18 May, 2022)**
### Features
* Added user Margin Accounts Manager.
* Added Home tabs for Margin Accounts Manager where specified next information (Name, Balance, Floating profit, Equity, Margin, Margin Level (%), Free Margin, Takers, Allow trade).
* Added TradingView connector (Trades, Quotes).
* Removed delete/edit buttons from the GUI (Positions tab).
### Changes
Freonted libraries updated.

## **Version 1.145 (11 May, 2022)**
### Features
* Added order execution price slippage.
### Changes
* Added support for a new .csv file format where time and date specified to import swap values for Risk Profile rules. Date and time in this case not applying. 

## **Version 1.143 (28 April, 2022)**
### Features
* Slippage column logic added.
### Changes
* Added logging of IP of the user who makes changes in the hub..
* Fixed error display if the hub failed to connect to the database.

## **Version 1.142 (19 April, 2022)**
### Features
* Delay column logic added.
* Added Slippage column to risk profiles rules.
### Changes
* Added pings/heartbeats for the gate.io maker.
* Added a popup if the risk profile rules are not saved.
* Fixed bug, inability of profile risk rules to trigger due to addition of delayed order execution logic .
* Added update to the list of available Binance Futures maker symbols.

## **Version 1.140 (01 April, 2022)**
### Features
* Added delay column to risk profile rules.
### Changes
* Fixed bug of wrong error display in case of entering incorrect values into profile risk rules.
* Fixed Hub Symbols highlighting in Advanced mode if no quotes are received.
* Fixed bug when executing orders in B-Book for quotes from Gate.io.
* Prohibited the ability to use space characters except space for fields that can be uploaded to TSV format.
* Changed the logic of filling settings FIX sessions on the makers and takers, if earlier in the case of settings ResetOnLogon and ValidateFieldsHaveValue issued an error, now the values are added automatically.
* Added additional logging if heartbeat is zero.

## **Version 1.139 (23 March, 2022)**
### Features
* Added creation of separate CSV files with quotes for each maker.
* Added alert if user increases margin rate in risk profile settings.
### Changes
* Fixed a bug with question marks when credit is deposited.
* Added matching of rules in risk profile with orders.
* Added reading order details from fix message.

## **Version 1.138 (18 March, 2022)**
### Features
* Added possibility to import swaps to risk profile using CSV file.
* Added Volume Step setting in Price Channels.
* Added preview, table display, after uploading a CSV file to the Price Channel.
### Changes
* Fixed filtering positions by symbol.
* Simplified calculation of the average price net - position.

## **Version 1.137 (14 March, 2022)**
### Features
* Added Cancel All GTC button for user with Margin rights.
### Changes
* Added timeout-lock for managers (providerManager) and for the core config record lock.
* Fixed bug of status polling for active GTC orders on Binance.

## **Version 1.136 (10 March, 2022)**
### Features
* Added TraderTools maker with FOK / IOC time in force.
### Changes
* The error output in the log in the case of time mismatch on the taker side and Hub.
* Added additional status check for active GTC orders on Binance maker.
* Added log output of symbol name, tickSize and LOT_SIZE for Binance maker.
* When adjusting a position on the margin account in the Home tab, it splits into A-Book and B-Book parts.
* Changed the visual part of updating the list of positions on the margin account.
* Removed question marks from the Margin Account column for TSV report on trades.
* Added a link to the support page in the GUI header.

## **Version 1.135 (3 March, 2022)**
### Features
* Quote filtration added in taker connection configuration .
### Changes
* Execution performance was optimized for the margin account.
* TSV reports now can be downloaded additionally for positions, orders and positions history.
* GTC partial order fills from Binance makers are now fully supported.
* bug fix: GTC orders were executed in b-book by their request price.

## **Version 1.134 (3 March, 2022)**
### Features
* New risk management rules were added into risk profiles - soon it will be possible to execute orders on the margin accounts according to their min / max volume, MT4 login’s and their instruments.
### Changes
* Order status request was added for active GTC orders on Binance makers.
* Extended logging during TSV import was added to monitor possible issues.
* Hub interaction with it's database was optimized.
* Full hub name is now visible only after successful user login.
* TSV backup file names were made more detailed.

## **Version 1.133 (16 Feb, 2022)**
### Features
* Active orders menu was added into margin account user GUI.

## **Version 1.132 (4 Feb, 2022)**
### Features
* Partial fills processing logic for GTC orders.

## **Version 1.130 (27 Jan, 2022)**
### Features
* Risk management logic (can't be seen in the GUI yet).
* GTC orders support for Takeprofit protocol.
### Changes
* bug fix: hub symbols priority was not working with Gate.io maker.
* bug fix: taker limit orders were rejected by the Hub according to it's book even in full a-book execution - now the Hub will send such orders to LP.

## **Version 1.129 (17 Jan, 2022)**
### Features
* GTC orders are supported now by Binance Spot and Futures makers.
* Maker Gate.io in quote-only mode. 

## **Version 1.128 (20 Jan, 2022)**
### Changes
* Bug fix: credit was included into balance.

## **Version 1.127 (11 Jan, 2022)**
### Features
* Credit funds now can be added or removed from the margin accounts.

## **Version 1.126 (29 Dec, 2021)**
### Features
* Incoming limit orders from takers now can be sent as GTC to OneZero maker (with LimitAsGTC setting enabled).
* Two new swap types suited for CFD products were added: 'by interest (open price) by quote currency', 'by interest (current price) by quote currency'.
### Changes
* Bug fix: partial fills were ignored for Integral maker.

## **Version 1.125 (24 Dec, 2021)**
### Changes
* Bug fix: VWAP price could be worse than limit price for b-book execution.
* Bug fix: color indication of margin level was not working in 'Margin Accounts' if 'Allow SO' was enabled.

## **Version 1.124 (22 Dec, 2021)**
### Features
* TSV backups are made now in the 'BackupTSV' folder in case of any changes of hub symbols, maker symbols, price channel rules or risk profile rules.
### Changes
* Faster book loading in margin account market watch.
* Bug fix: fixed indication of old quotes in 'Hub Symbols' menu.

## **Version 1.123 (15 Dec, 2021)**
### Features
* Quotes logging for FIX API can be disabled now.
* Added OrderStatusRequest on logon for Xenfin API.
### Changes
* RAM usage optimization.
* Bug fix: open position could not be edited if margin account currency was different from quote currency of open position.

## **Version 1.121 (9 Dec, 2021)**
### Features
* New supported maker API: Integral (Velocity).
### Changes
* Open Volume, Open Price, Close Price, Close Volume, Conversion Rate are shown fully now in 'Positions History' and position details.
* Rate limits are now balanced between makers for Binance (both Spot and Futures).
* Bug fix: removing hub symbols could cause an error if new makers were created recently.
* Bug fix: margin account users could see execution notifications from other margin accounts.
* Bug fix: expected margin calculation was corrected to avoid accidental rejects due to unsuccessful margin checks.
* Bug fix: subscribing to Binance Spot to non-existent symbol could cause an error.

## **Version 1.120 (30 Nov, 2021)**
### Features
* New supported maker API: Xenfin (Velocity).

## **Version 1.119 (23 Nov, 2021)**
### Changes
* All configuration changes are now registered in the full log.
* Orders can now be found faster in the database with filters applied by order level, CID and taker name.
* Performance optimization for quotes processing and margin calculation.
* Bug fix: price channel or maker symbols update could cause a freeze of the hub.
* Bug fix: buy deals in the 'close volume' column in positions history were shown as negative values (visual bug).

## **Version 1.118 (9 Nov, 2021)**
### Features
* Position snapshots were added into daily equity reports.
### Changes
* Subscriptions were limited to 5 per second for Binance Futures maker to avoid a ban from Binance.
* Zero profit records are now shown in 'Account History'.
* Margin account balance now will be fixed immediately if any positions were deleted in 'Positions History'.

## **Version 1.117 (29 Oct, 2021)**
### Features
* Exante (quotes only) maker is added.
### Changes
* Time widget was added in filters to simplify time input.
* Bug fix: javascript libraries were added into 'wwwroot' folder to avoid GUI loading problems.
* Bug fix: taker connection status could be incorrect if only quote or trade was disconnected.
* Bug fix: deleted hub symbol could cause an error if it was present in 'Symbol Overrides' rules for any risk profile.

## **Version 1.114 (7 Oct, 2021)**
### Changes
* Bug fix: profitable positions could be opened on the margin account with zero balance.

## **Version 1.113 (5 Oct, 2021)**
### Features
* New supported maker API: GCEX.
* Incoming market orders from takers now can be sent as GTC to OneZero maker (with MarketAsGTC setting enabled).
### Changes
* New metric added: rejects per second.
* Rate limits for Binance Spot maker API now can be ignored, if necessary.
* Rate limits for Binance Futures maker API now can be ignored, if necessary.
* Information about zero positions is not requested now from Binance Futures to decrease log size.
* Information about zero assets is not requested now from Binance Spot to decrease log size.
* Warning message in case if user tries to delete active hub symbol is more detailed now.
* Bug fix: closed positions open and close time now can be modified without errors.

## **Version 1.112 (23 Sept, 2021)**
### Changes
* Top of the book quotes now recorded in .csv format (if SaveQuotesToLog setting is enabled for the maker).
* Full taker configuration is recorded in the fix log now, if modified.
* Bug fix: VWAP filling price from Binance Spot maker now calculated correctly.
* Bug fix: time values are accepted without errors now in databases filters.

## **Version 1.111 (17 Sept, 2021)**
### Features
* New supported maker API: Binance Spot.
### Changes
* JavaScript's libraries now included in .exe file.
* Profit in position details now has the same number of digits as in the price channel for an instrument.
* Bug fix: long book loading in 'Hub Symbols' -> 'Book' menu.

## **Version 1.110 (3 Sept, 2021)**
### Features
* New columns in equity reports: Balance, Profit, Margin, Margin Level, Free Margin.
* TSV reports export in equity reports.
### Changes
* Requirement to enter milliseconds removed from databases time filters.
* Bug fix: long orders execution for Binance Futures maker API.
* Bug fix: fixed exception on pressing 'Takers' and 'Takers Total' columns names in Home tab.
* Bug fix: active full b-book orders are canceled now after the Hub restart.

## **Version 1.109 (27 Aug, 2021)**
### Changes
* Bug fix: no data in active orders and positions GUI pages.
* Bug fix: errors on order opening by margin account users.

## **Version 1.108 (26 Aug, 2021)**
### Changes
* Bug fix: missing icons in execution tree diagrams for orders and deals.

## **Version 1.107 (26 Aug, 2021)**
### Features
* New supported Maker API: Match-Trade.
* 3-days swaps now can be added for each instrument individually.
* Market orders now can be opened by margin account users.
### Changes
* Hub browser tab now includes folder name for easier differentiation between several Hub's.
* ASP.net libraries update.
* Full b-book orders now filled by the Hub with volume-weighted average price.
* Bug fix: fixed duplicates in equity reports.
* Bug fix: fixed exception on pressing 'Takers' and 'Takers Total' columns names in Home tab.

## **Version 1.106 (19 Aug, 2021)**
### Changes
* Position open price on the margin account was restricted to the same number of digits as in the price channel of an instrument.
* Old quotes indication added (quotes older than 60 seconds will be highlighted by the red color in 'Hub Symbols').
* The exact name of an instrument will be shown now, if the imported TSV spreadsheet in 'Symbol Overrides' has non-existent hub symbols.
* Hub browser tab will now include the folder name for easier differentiation between several Hub's in one browser.
* Hub logo in the browser now leads to the 'Home' tab.
* Bug fix: special symbols as ' are now processed correctly by the 'Maker Text' button in the 'Orders' database (button did not work in some cases previously).

## **Version 1.105 (6 Aug, 2021)**
### Features
* Read-only user role (this user see all settings and data, but can’t make any changes) ‘TSV report’ button to Account History tab.
* New tabs to margin user role: Account History and Equity Report.
* New supported Maker API: Binance Futures (full support: trade and quotes).

### Changes
* Bug fix: margin level for zero balance margin account is calculated correctly now.

## **Version 1.104 (30 Jul, 2021)**
### Features
* PrimeXM maker API: optional tag 1 (Account) added to new order request message (35=D) now it’s possible to set time in filters: Orders, Deals, Position History, Account History, Equity Reports.
### Changes
* Now volume conversion rate to USD for deal is possible not only from base currency, but from quoted currency too.

## **Version 1.103 (23 Jul, 2021)**
### Features
* OneZero maker API: optional tag 115 (OnBehalfOfCompID) added to new order request message (35=D).
### Changes
* Search filters validations (Orders, Deals): volume values can’t be negative.
* Bug fix: rejection b-book FOK order if price provider is Kraken - now orders successfully execute in b-book.

## **Version 1.102 (21 Jul, 2021)**
### Features
* New supported Maker API: Binance Futures (quotes only).

## **Version 1.101 (2 Jul, 2021)**
### Changes
* Version control was added to avoid unnecessary database migration during an upgrade.
* Number of Hub files was significantly decreased for easier installation and upgrading.
* Bug fix: exception occurred during limit order execution in case of partial B-book by the Hub.

## **Version 1.100 (25 Jun, 2021)**
### Changes
* Bug fix: IOC orders are now sent with MinQty = 0 to PrimeXM and OneZero makers.

## **Version 1.99 (25 Jun, 2021)**
### Features
* MarketAsIOC parameter was added for PrimeXM and OneZero makers to ensure the usage of the full book on LP (details can be found here).
### Changes
* A warning message will now appear in the log, if FOK order was filled partially by the liquidity provider.
* A warning message will now appear in the log, if a limited order was filled with negative slippage by the liquidity provider.
* Bug fix: REST API maker sessions (like Kraken) were started twice, causing an error.
* Bug fix: exception occurred if a new instrument was added for Kraken maker API.

## **Version 1.98 (18 Jun, 2021)**
### Changes
* Bug fix: error log now won’t be duplicated in case if errors found in several logs (full and fix, for example).
* Bug fix: makers and takers names are now correct in the FIX logs.

## **Version 1.97 (16 Jun, 2021)**
### Changes
* Negative swap values can now be set.

## **Version 1.96 (10 Jun, 2021)**
### Changes
* Nlog logging libraries were replaced with Serilog (configuration settings can be found here).
* Each log type (full/fix/quotes/alpaca/kraken/okcoin/error) now recorded in a separate log for easier navigation and troubleshooting.
* Bug fix: business message rejects are now processed correctly for cTrader maker API.

## **Version 1.93 (20 May, 2021)**
### Features
* Equity reports are now recorded in 'Databases' -> 'Equity Reports' at the time of 'EOD offset' configured in the risk profile.
### Changes
* Comments in the 'Account History' records are now hidden under the button 'Show text'.
* Bug fix: redundant information was removed from the error notifications.
* Bug fix: equity reports are now recorded by 'EOD offset' even if there are no swaps configured.

## **Version 1.92 (19 May, 2021)**
### Features
* New supported Maker API: cTrader FIX API for Flowbank. 
### Changes
* Margin account name in addition to margin account ID is recorded now in equity reports in the logs.
* Equity reports in the logs now have a readable time format.
* 'Swap UTC Midnight Offset' renamed to 'EOD Offset' in the 'Risk Profiles' settings.
* Price channel rules menu was optimized for faster loading.
* Bug fix: adjust positions window now shown at the center of the screen.

## **Version 1.91 (10 May, 2021)**
* Feature:
* Swaps with an adjustable EOD offset added.
* Bucket added to keep volume in B-book until defined limit is reached and then send all collected volume to the liquidity provider.
### Changes
* Equity reports are now recorded to the log at the time of EOD set in the risk profile.
* Price channel rules menu optimization for faster page loading.

## **Version 1.90 (1 May, 2021)**
### Changes
* 'USD volume' column added in the 'Deals' database.
* 'Equity Reports' submenu added in the 'Databases' menu.
* Hub symbols with indices now will be shown on separate rows in the 'Home' menu instead of netting with plain symbols.
* Pagination was added for all databases for easier search.

## **Version 1.89 (27 Apr, 2021)**
### Features
* New supported Maker API: Alpaca (full support, previously long only trades were supported).
* New supported Maker API: FIX API for OKCoin. 
### Changes
* Market watch quotes for the 'MarginAccount' role user now include the markup from the price channel attached to this margin account.
* Bug fix: orders with the status 'Cancelled' now filtered correctly without showing orders with other statuses.

## **Version 1.88 (16 Apr, 2021)**
### Features
* One margin account now can be associated with multiple 'MarginAccount' users.
### Changes
* Users logins and passwords, base and quote currencies now can contain only up to 20 characters.
* Bug fix: maker symbol in maker's rules could be mistakenly processed only by one rule, even if there were several rules for identical maker symbols (associated with different hub symbols).
* Minor bug fixes and improvements.

## **Version 1.86 (13 Apr, 2021)**
### Features
* Swaps settings added for risk profiles (GUI only, full functionality will be available in the upcoming releases).
* Bucket settings added for risk profiles (GUI only, full functionality will be available in the upcoming releases).
### Changes
* Minor bug fixes and improvements.

## **Version 1.85 (03 Apr, 2021)**
### Features
* Possible active makers now can be restricted by the priority list for each hub symbol.
* Market watch added for the 'MarginAccount' user role.
* 'Home' menu reworked to show total open positions for each taker separately.
* Makers and takers connection settings templates now can be generated automatically for easier configuration.
### Changes
* Margin account without a risk profile set will now reject trades
* Loading speed was improved during an initial startup.
* Minor bug fixes and improvements.

## **Version 1.84 (15 Mar, 2021)**
### Features
* Top of the book for each FIX API maker now can be recorded in a separate log file.
### Changes
* Minor bug fixes and improvements.

## **Version 1.83 (5 Mar, 2021)**
### Features
* 'Allow Trading' setting was added for margin accounts to allow or disallow trading.
* MetaTrader 4 account’s ID display in the Hub database for orders, which were sent by MT4 Kloshira taker with API = Takeprofit (for easier execution inspection).
### Changes
* Margin account currency now can't be changed, if it has open positions or the balance is not 0.
* Bug fix: profit was not shown in the database for closed positions.
* Bug fix: closed positions could not be edited.
* Minor bug fixes and improvements.

## **Version 1.82 (28 Feb, 2021)**
### Features
* Commissions now can be set in risk profiles.
* Maximum depth for subscription now can be configured in 'Connection configuration' for FIX API makers.
* New metrics are collected now by the Hub for Prometheus / Grafana integration - average execution delay.
### Changes
* Bug fix: active orders could not be canceled in some cases.
* Minor bug fixes and improvements.

## **Version 1.81 (16 Feb, 2021)**
### Features
* Order processing speed optimization: 7000 trades per second as the peak volume, 500 trades per second as the constant volume.
### Changes
* Bug fix for IOC partial execution due to the volume step setting, when active orders could stuck in 'Databases' -> 'Active Orders'.
* Accounts with the role 'Manager' now can't delete or edit positions.
* Minor bug fixes and improvements.

## **Version 1.79 (4 Feb, 2021)**
### Features
* The time of the last quote arrival is now shown in the "Aggregated Instruments" menu.
### Changes
* Minor bug fixes and improvements.

## **Version 1.77 (20 Jan, 2021)**
### Features
* New supported Maker API: Alpaca (long account support only).
### Changes
* Change in the logic of fill or kill orders execution if there is not enough volume in the Hub's book - now the Hub will not reject such orders itself, but will send them to the liquidity provider anyway.
* Minor bug fixes and improvements.

## **Version 1.76 (26 Dec, 2020)**
### Features
* New metrics are collected now by the Hub for Prometheus / Grafana integration to track makers / takers status and errors quantity.
* "allow stopout" option for margin accounts to avoid accidental stopouts.
* "digits" settings for new price channel symbols are now taken automatically from respective aggregated instruments.
### Changes
* Bug fix: fixed subscriptions/unsubscription problem for Takeprofit protocol.
* Column order in .TSV report is now the same as in databases -> deals menu for easier navigation.

## **Version 1.74 (4 Dec, 2020)**
### Features
* Open positions now can be edited or removed.
* Margin account status now updating in real time for margin account user.
* Rejection stats available for the last 10 minutes for each maker.
### Changes
* Bug fix: for FOK execution the Hub could send to LP more volume than is available in the book.
* Bug fix: some balance entries could be missed causing missing profits on the margin accounts.
* Minor bug fixes and improvements.

## **Version 1.73 (27 Nov, 2020)**
### Features
* Maker with the highest priority (if configured) will be used to receive quotes / execute trades. In case of its disconnection, the next maker in the priority list will be used. 
### Changes
* Margin accounts positions now include taker's markup (if it is set).
* Minor bug fixes and improvements.

## **Version 1.69 (9 Sep, 2020)**
### Features
* New type of user for authorization: margin account manager (currently available: administrator and manager). New users with their own credentials will be able to check active/closed positions and margin account status: balance, equity, margin, marginLevel, free margin.
* New aggregation mode: simple. In this mode, the trade will be executed on one maker fully with the best price available.
### Changes
* New supported Maker API: Kraken.
* Minor bug fixes and improvements.

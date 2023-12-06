# Takeprofit Hub

## Version 1.271 (4 December, 2023)
### Changes
* Hints when hovering the buttons are removed.
* Minor GUI changes.
* 

## Version 1.277 (3 December, 2023)
### Changes
* Minor GUI changes.
* TSV import/export logic is improved: now import or export is amde as atomic operation.
* 

## Version 1.268 (27 November, 2023)
### Changes
* Trade details page is migrated to Syncfusion frontend framework.
* 

## Version 1.266 (23 November, 2023)
### Changes
* Trade details page is migrated to Syncfusion frontend framework.
* 

## Version 1.265 (21 November, 2023)
### Changes
* Position Reports table is migrated to Syncfusion frontend framework.
* Users table is migrated to Syncfusion frontend framework.

## Version 1.264 (19 November, 2023)
### Changes
* Market watch is added for Margin account (read only) role.

## Version 1.263 (17 November, 2023)
### Changes
* Margin account (read only) role is added.

## Version 1.259 (16 November, 2023)
### Changes
* Now it is poossible to change the style of hub's GUI by changing inner css file (css file is not hardcoded anymore).

## Version 1.245 (11 November, 2023)
### Changes
* Margin account positions table is migrated to Syncfusion frontend framework.
* Margin accounts table is migrated to Syncfusion frontend framework.

## Version 1.244 (9 November, 2023)
### Changes
* FIX unsubscription logic is improved: now the hub does not check the existence of the symbol before unsubscription.
* 

## Version 1.242 (6 November, 2023)
### Changes
* Incorrect FIX taker templates are fixed.
* 

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
* 

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
* Added filtration for syntactic symbols.
* Added T4B acceptor
* Added “Execution time” column in orders table.
* Added “Order price slippage” column in orders table.

## **Version 1.202 (9 June, 2023)**
### Features
* Added working logic for syntactic symbols.
* Added a new index (order_time_stamp_idx) to the internal_order table. (internal change in database)
### Changes 
* Minor displaying bugs fixed.
* Fixed loading error on homepage.
* MakerExecutedPrice, TakerRequestedPrice, MakerTradeId, TradeDate, MakerSlippage columns were removed from margin account report

## **Version 1.197-1.201 (1 June, 2023)**
### Features
* Added report to margin account in web GUI.
* Added logic of margin account report generation.
* Added fields for syntactic symbols in web GUI.
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

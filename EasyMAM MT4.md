# EasyMAM MT4

## **Version 4.31-4.32 (20 Dec, 2023)**
### Changes
* Added a check if an order is open or closed if the error "Failed to execute TradeTransaction" is received.

## **Version 4.29-4.30 (24 May, 2023)**
### Changes
* Added “Incentive rollback function”.
* Added “Batch Incentive rollback function”.
* Fixed errors related to incorrect work of “Incentive rollback function”.

## **Version 4.27-4.28 (14 Mar, 2023)**
### Changes
* Added clearing the cache from the information about the rest connection, for the correct GUI work.

## **Version 4.26 (10 Mar, 2023)**
### Changes
* Made internal code changes related to optimization.

## **Version 4.25 (14 Feb, 2023)**
### Changes
* Config file migrated from XML to JSON format.

## **Version 4.23-4.24 (16-21 Dec, 2022)**
### Changes
* Fixed reset value of incentive for accounts in GUI.  

## **Version 4.22 (30 Nov, 2022)**
### Changes
* Updated authorization and loading page in the web GUI.  
* Added “AllowIncentivePayment” parameter in web GUI.
* Added confirmation for detach in GUI.
* Added information in log about a “FATAL” error in case of incorrect filling of the config file. 

## **Version 4.20-21 (23 Nov, 2022)**
### Changes
* Fixed a bug due to which the application doesn't “start” and doesn't “stop” in  Windows services.
* Fixed “balance fix” for slaves removed from the server, which caused an error of discrepancy between the balance of the master and slaves.
* Information about errors in case of incorrect filling of the config file was transferred to EventViewer from the application log file.

## **Version 4.18-4.19 (3 Nov, 2022)**
### Changes
* Added visual changes to web GUI.
* Some libs have been added to the application due to the absence of which the application could not start.

## **Version 4.17 (1 Nov, 2022)**
### Changes
* Information about "start step" and “complete step” added in log file.
* Added more detailed information about the server to the log file when a “FATAL” error is detected.
* Changed message in log file in case of calculation incentive for not existing incentive acc.
* Added “batch” buttons for making operations with several slave accounts in web GUI.

## **Version 4.16 (21 Oct, 2022)**
### Changes
* Added web GUI.
* Added “RestHost” and “RestPort” parameters for web GUI connection. 

## **Version 4.15 (7 Sep, 2022)**
### Changes
* Now EasyMAM writes a message in the log file when it can't find the deleted orders on the MT4 server:
"Can't request lost orders from MT4: {lost orders list}. Perhaps orders have been deleted".

## **Version 4.12 (4 Aug, 2022)**
### Changes
* After the application stops working due to a disconnection from the server, it will be automatically restarted.

## **Version 4.11 (15 July, 2022)**
### Changes
* Changed error logging when connecting to the server from "FATAL" to "ERROR".

## **Version 4.10 (06 Jun, 2022)**
### Changes
* “Default” distribution mod value from the master menu in GUI was removed.
* Fixed button fonts in GUI.
* Text field of the slave attach window in GUI has been increased to 50 symbols.
* Fixed a bug due to which the application did not start when the Internet connection was broken.

## **Version 4.09 (27 Jan, 2022)**
### Changes
* Fixed a bug related to incorrect distribution of deals.

## **Version 4.08 (20 Jan, 2022)**
### Changes
* Fixed a bug that occurred if you remove the account from the “Master” or “Slave” group.

## **Version 4.02-4.06 (17 Nov, 2021)**
### Changes
* Fixed GUI bug, related to Metatrader API crash when receiving email notification. 
* Adjusted PumpingSwitch “CLIENT_FLAGS_HIDEMALL” parameter in the code.

## **Version 4.01 (31 Aug, 2021)**
### Changes
* Reconnection bug after “CANNOT_CONNECT” fatal error was fixed.
* Attach/detach loading bug in GUI was fixed.

## **Version 3.122 (19 Aug, 2021)**
### Changes
* Pumping data is excluded from EasyMAM working logic.
* Memory leak is fixed.

## **Version 3.120 (6 Aug, 2021)**
### Changes
* The minor connection bugs are fixed (data transfer between EasyMAM application and TPT License server is improved).
* The minor bugs of logging are fixed.

## **Version 3.118 (23 Jun, 2021)**
### Changes
* Additional data check is added to EasyMAM (it double checks if the balance of slave accounts is valid).

## **Version 3.117 (21 Jun, 2021)**
### Changes
* The bundle is made as one .exe file (instead of many different files).
* Nlog logger is replaced by Serilog logger.
* EasyMAM is rebuilt with .NET Core instead of .NET Framework.
* GUI typos are fixed.

## **Version 3.116 (16 Jun, 2021)**
### Changes
* The text about EasyMAM service stopping is added to the log file.

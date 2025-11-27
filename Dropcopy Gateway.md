# Dropcopy Gateway

## Version 2025.11.18.661 (20 November, 2025)
### Changes
* .xml files have been replaced with .dat files for backup compatibility.
* Log files are now stored inside a single log folder. Previously they were divided between different folders.
* BadConfiguration error now passed to FATAL level.
* If connector starts with any errors, the gateway shuts down.

## Version 2025.11.14.684 (14 November, 2025)
### Changes
* The mechanism of cache initialization is improved: the cache will be initialized before processing requests or any other operations. 

## Version v2024.12.10.689 (10 December, 2024)
### Changes
* MT5 Gateway API has been updated to v4731.

## Version 1.07 (3 March, 2023)
### Changes
* Deleted stacktrace from error about unsuccessful connection.
* Added ability to set several gateways from one instance.


## Version 1.06 (22 February, 2023)
### Features
* Added partially filled active orders.
* Added sqlite database to store execution.
### Changes
* Fixed error while receiving 35=8 message.


## Version 1.03 (13 February, 2023)
### Changes
* Fixed bug incorrect handling with partially filled orders.

## Version 1.02 (25 October, 2022)
### Features
* Added support for several dropcopy sessions.

## Version 1.01 (21 October, 2022)
### Changes
* Product has been created.

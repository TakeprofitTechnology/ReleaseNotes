# Drawdown Limit MT4

## Version 25.06.27.44 (27 June, 2025)
### Changes
* Added readable falal log message for license exceptions.

## Version 24.07.23.27 (23 July, 2024)
### Features
* It is possible now to configure the plugin via Web GUI configurator.

## Version 1.02 (30 November, 2023)
### Changes
* Merged the code bases od Drawdown Limit MT5 and Drawdown Limit MT4.
* Fixed calculation of the DailyLossLimitPercent parameter: MeasuredDailyLoss is now recalculated every day.

## Version 1.01 (16 November, 2023)
### Changes
* Fixed a bug with closing pending orders in the flat balance profit check mode.

## Version 1.00 (14 November, 2023)
### Changes
* Created the first version of the plugin with the followinf parameters: TotalDrawdownLimitPercent, DailyDrawdownLimitPercent, ProfitCheckMode, HighWatermarkMode, IntegrationWebhook, ProfitLimitPercent, FirstLimitsCalculation, LossLimitPercent, DailyLossLimitPercent.

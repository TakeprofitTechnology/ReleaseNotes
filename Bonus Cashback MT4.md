# Bonus Cashback MT4

## Version 26.09.28.74 (30 September, 2026)
### Changes
* The plugin now refuses to start if a setting is missing or invalid. The Administrator shows a red status naming the setting.
* A bad configuration pushed while the plugin is running is now rejected. The plugin keeps paying cashback with the previous settings.
* The cashback percentage must now be a plain number. Values like "10%" or "10,5" are refused, so check this setting before upgrading.
* The error for an invalid cashback mode now shows the list of allowed values.

## Version 25.01.21.42 (21 January, 2025)
### Features
* Added the option to set a cashback mode;
* Added the option to set a custom comment for balance operations;

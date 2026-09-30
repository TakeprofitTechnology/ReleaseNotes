# Email Notifier MT4

## Version v26.09.28.59 (29 September, 2026)
### Changes
* If a setting is missing or invalid, the plugin now refuses to start. The status badge and a FATAL line in the journal name the wrong setting.
* A bad configuration pushed from the Administrator is now rejected. The plugin keeps running on the previous valid configuration.
* Misspelled values in the notification interval and the "use TPT Mailgun account" setting are now rejected. Before, they were silently ignored.
* The notification interval can't be more than 44640 minutes (31 days).
* The webhook must be a full address that starts with http:// or https://.
* The sender address must be a valid email address, for example alerts@broker.com or Broker Alerts <alerts@broker.com>.
* Spaces around a value pushed from the Administrator are now removed, the same as at startup.
* If the notification interval is not set, the journal now says the 10-minute default is used.
* If an account has no email on its card, the plugin now writes an ERROR line that names the account.
* Before upgrading, check Settings.ini. Values that were accepted before, such as "15m", an interval over 44640, a webhook without http(s):// or a sender that is not an email address, will now stop the plugin from starting.

## Version v26.05.06.49 (8 May, 2026)
### Changes
* Fixed the issue with parameter 'Groups=*' which can led to virtual memory leak and server crash. Now plugin scans only accounts that actually have an open trade.

## Version v24.12.16.39 (16 December, 2024)
### Changes
* Optimization in memory consumption;

## Version v24.10.22.35 (22 October 2024)
### Changes
* Logging has been extended with account number id and type of message (SO/MC);

# Hedge Locker MT5
## Version v26.08.10.53 (11 August, 2026)
### Features
* Decisions on position closes are now written to the MT5 server journal (Manager terminal → Servers > Journal, Event type "API") — one self-contained line per attempt showing whether the close was ALLOWED or BLOCKED, the login, group, symbol, action, volume, open buy/sell volumes, the hedge ratio, the rule line that decided and its settings, and the reason for the decision.
* Only closes matched by a rule reach the server journal — closes that match no rule and exempt closes such as Stop Loss are recorded in the plugin log only, so the journal is not flooded with routine traffic.
## Version v26.07.15.46 (17 July, 2026)
### Features
* Initial version of the plugin has been created.

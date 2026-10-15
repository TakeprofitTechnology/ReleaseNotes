# Takeprofit Demo Portal

## Version 2026.10.14.394 (15 October, 2026)
### Features
* The portal and all demos can now work over HTTPS. HTTPS is off by default and is turned on in the settings file.
* The certificate comes from Let's Encrypt and renews by itself. A company certificate can be used instead.
* With HTTPS on, the old http address redirects to https.
* The admin's Stand page shows the certificate's expiry. It warns when the certificate is expired, untrusted, does not cover the demos or has less than 20 days left.
* Social Trading demos now have a REST API and a Swagger link, like Hub and PAMM.
* Social Trading demos now run in a limited demo mode. Only the demo logins admin, 1000, 1001 and 1002 can sign in, and registration is closed.
* In Social Trading demos, servers, users, passwords and trading accounts cannot be added or deleted. These buttons are disabled with the hint "Disabled in demo mode".
* Social Trading demo data is now kept when the demo restarts. Old trades are compacted to keep the demo small.
* The admin's Demos page shows how much disk space each demo uses. Demos over the "Large demo, MB of data" setting (200 by default) are marked.
* The admin can now reset a demo or restart it with compact. Compact keeps the data but shrinks old trading history. Both ask for confirmation.
* The owner's Restart button is now called Reset.
* The login page warns that phone sign-in works only with a verified number. The profile shows that phone sign-in is blocked until the number is verified.
### Changes
* Phone sign-in now works only with a verified number. Before, a second account with the same unverified number broke phone sign-in for both.
* Sign-in no longer shows whether an account exists by how long it takes to answer.
* The demo limit now holds when several visitors start a demo at the same moment. The extra visitors see "No free demo slots".

## Version 2026.10.10.711 (12 October, 2026)
### Changes
* Sign-in no longer shows whether an account exists. A locked-out account now gets the same "Invalid login or password" message as an unknown login.

## Version 2026.10.7.897 (8 October, 2026)
### Features
* First release of the portal. Visitors register, verify their phone by SMS and start their own demos of Hub, Social Trading and PAMM.
* One demo per product per account. Only its owner and the admin can open a demo.
* The admin can manage users, demos and portal settings. Settings apply without a restart.
* Each demo gets its own passwords for its demo logins. The product's sign-in page shows them in a "Demo logins" panel.
* The owner can restart a demo. All data in the demo is reset; the address, remaining time and passwords stay the same.

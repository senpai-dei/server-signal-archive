---
id: 222976
title: "CorePanel 1.13 is out - free up to 20 sites"
date: "2026-11-05T21:38:36+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/222976/corepanel-1-13-is-out-free-up-to-20-sites"
---
# CorePanel 1.13 is out - free up to 20 sites
**Link:** [Original Thread](https://lowendtalk.com/discussion/222976/corepanel-1-13-is-out-free-up-to-20-sites)

CorePanel 1.13 is out, for RHEL, AlmaLinux and Rocky 8–10. With this release every edition, the free one included, gives you two panels: one for you and one for each of your customers.

What the admin sees
-------------------

![](https://www.corepanel.net/_astro/admin-panel-classic-blue.C2cBj3ce_Z1VPdbr.webp)

[Open the admin demo](https://demo.corepanel.net/login?demo=admin&theme=classic-blue&utm_source=lowendtalk&utm_medium=offer&utm_campaign=offer-nov26&utm_content=demo-admin) (demo runs on mock data)

Accounts and hosting packages, domains, mail, DNS, SSL, the WAF and firewall, backups and cPanel imports. A PHP version per site, 7.4 to 8.4: the PHP a fresh install ships is already patched against PHP2Shell (CVE-2026-109618/109619), every installed version gets security updates daily, and an unpatched one is flagged. From any account you can log in as that customer. PHP versions from 5.4 are also available.

What the client sees
--------------------

![](https://www.corepanel.net/_astro/client-panel-classic-blue.JnoAe-YN_Z1CeOBI.webp)

[Open the client demo](https://demo.corepanel.net/login?demo=client&theme=classic-blue&view=icons&utm_source=lowendtalk&utm_medium=offer&utm_campaign=offer-nov26&utm_content=demo-client) (demo runs on mock data)

Only their own account: sites, a file manager, mailboxes and forwarders, DNS, databases, SSL, FTP, SSH and SFTP in a jail, cron jobs, backups and the PHP version of each site. On Pro and Business, WordPress too. Every mailbox also has its own page using webmail. with usage, auto-reply, forwarding and recent sign-ins.

It fits what a hosting business already runs: a native WHMCS module plus a WHM-compatible API on :2087, cPanel account import and export (restorepkg -ready) and standard IMAP/POP3/SMTP.

**CorePanel 1.13 runs our own production, as every release does: all our sites, www.corepanel.net included, our company mail, our WHMCS and all our corporate sites**

Pricing, per server, not per account
------------------------------------

* **Personal — free.** Up to 20 websites. Client panel, mail, DNS, MariaDB, PHP, free SSL, local backups, the full WAF in blocking mode and brute-force blocking.
* **Pro — $14.90/mo.** Up to 50 websites. WHMCS, resellers, suspension, WordPress in your customers' panel, remote backups to S3 or SFTP, page cache.
* **Business — $24.99/mo.** Same as Pro with no website cap, plus priority support.

**21-day trial of Pro or Business at your first login**, no card.

Checkout prices by country, so many places pay less.

**Requirements:** RHEL, Alma or Rocky 8, 9 or 10, x86\_64, root, 2 GB RAM. SELinux stays enforcing. No Ubuntu or Debian yet.

Migrating from cPanel?
----------------------

It’s easy: corepanel-transform converts your cPanel server to CorePanel without any account migrations, DNS changes or anything like that, keeping your accounts, domains, email accounts and passwords exactly where they are.

Details: [https://www.corepanel.net/transform](https://www.corepanel.net/transform?utm_source=lowendtalk&utm_medium=offer&utm_campaign=offer-nov26&utm_content=transform "https://www.corepanel.net/transform")

Security, on every edition
--------------------------

The full WAF blocks on every site (SQL injection, XSS, path traversal), with a WordPress rule set you can switch on and an attack log per domain. Password guessing against the panel, mail and FTP ends in a firewall ban, and the SSH guard bans attackers from the SSH port, root included. Every account is isolated: a 0700 home, its own PHP-FPM pool, its SSH in a jail, and SELinux enforcing on the whole server.  
...

Documentation: [https://www.corepanel.net/docs](https://www.corepanel.net/docs?utm_source=lowendtalk&utm_medium=offer&utm_campaign=offer-nov26&utm_content=docs)  
Pricing: [https://www.corepanel.net/pricing](https://www.corepanel.net/pricing?utm_source=lowendtalk&utm_medium=offer&utm_campaign=offer-nov26&utm_content=pricing)  
Installation: [https://corepanel.net/docs/getting-started](https://www.corepanel.net/docs/getting-started?utm_source=lowendtalk&utm_medium=offer&utm_campaign=offer-nov26&utm_content=getting-started)

I'm around to answer questions here.

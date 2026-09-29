---
id: 221543
title: "CorePanel - a safe and modern web hosting control panel"
date: "2026-09-29T09:07:07+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/221543/corepanel-a-safe-and-modern-web-hosting-control-panel"
---
# CorePanel - a safe and modern web hosting control panel
**Link:** [Original Thread](https://lowendtalk.com/discussion/221543/corepanel-a-safe-and-modern-web-hosting-control-panel)

Hello LowEndTalk 👋

We're Pyxsoft. You may not know the name, but if you've ever rented a cPanel server from  
a provider running **pxShield**, our WAF has been sitting in front of your Apache since 2020.

We got tired of shipping products *around* a control panel, so we wrote our own.

![](https://www.corepanel.net/social/dashboard.png)

**CorePanel**  
is a hosting control panel for RHEL 8/9/10, AlmaLinux and Rocky — and the part LET will care  
about: **the web server is ours too**. Not Apache with a config generator on top. Not nginx  
with templates. Our own server, our own WAF, in one static binary.

**Install:**  
In a new server, as root:

```
curl -fsSL https://get.corepanel.net/install.sh | bash
```

**Live demo:** [https://demo.corepanel.net](https://demo.corepanel.net?utm_source=lowendtalk "https://demo.corepanel.net")  
**Site:** [https://www.corepanel.net](https://www.corepanel.net?utm_source=lowendtalk "https://www.corepanel.net")   
**Docs:** [https://www.corepanel.net/docs](https://www.corepanel.net/docs?utm_source=lowendtalk "https://www.corepanel.net/docs")

---

🎁 LET GIVEAWAY: A YEAR OF PRO FOR 10 REAL SERVERS
-------------------------------------------------

We want 10 people who actually use it, not 10 installs that get wiped on Friday.

1. Install CorePanel and pick the **14-day Pro trial** at first login.
2. Put something real on it: at least one account with a working site.
3. Reply here with `corepanel --version` and **one honest line**: the best thing, the worst thing, or what broke.
4. **PM me** the server's public IP and a screenshot of your Accounts list. We turn your trial into a **full year of Pro**.

The first **10 LET members** win, one server each. Entries close **October 31** or when we reach 10.

**Hosting customers?** Pro is for running your own sites. It has no client area, so your customers can't log in. If you're selling hosting, you want **Business**: say so in your PM and that's the year you get.

**Didn't make the 10?** Nothing to do. When the trial ends, your server drops to **Personal** on its own. That's free forever, up to 20 sites, and everything you set up keeps running.

---

WHAT YOU ACTUALLY GET
---------------------

* **CoreHttpd** — our web server. HTTP/1.1, **HTTP/2 and HTTP/3 over QUIC on by default**, nothing to enable.
* **Real .htaccess support** — mod\_rewrite, deny rules, password-protected directories — plus a per-site report of any line it *didn't* apply. Your WordPress users learn nothing new.
* **WebP conversion on the fly** — no plugin, no build step, no "optimizer" subscription.
* **Real Early Hints (HTTP 103)** — learned from the page itself and replayed. Nothing to  
  configure. Show me the other panel that does this.
* **PHP 7.4 → 8.5**, FastCGI, **one FPM pool per account**. PHP is never executed inside  
  the server process.
* **True isolation** — homes are `0700`, dedicated pools, and the panel's own daemons run **unprivileged, confined in their own SELinux policy, with SELinux enforcing**. We ship the policy in the RPMs. Nobody here has to type `setenforce 0` to make our panel work.
* **Mail** (Postfix + Dovecot + rspamd), **DNS** (PowerDNS), **MariaDB**, **FTPS & SFTP with SSH keys managed in the panel and jailed to the home**.
* **Free SSL** issued and renewed by the server, every edition.
* **Local scheduled backups**, every edition.

---

THE FREE TIER IS NOT A TEASER
-----------------------------

Read the free column twice:

|  | **Personal (Free)** | **Pro** | **Business** |
| --- | --- | --- | --- |
| Websites | **20** | ∞ | ∞ |
| CoreHttpd + HTTP/3 + Early Hints + WebP | ✅ | ✅ | ✅ |
| **Full WAF — SQLi, XSS, WordPress, path traversal — BLOCKING** | ✅ | ✅ | ✅ |
| Host firewall + **automatic brute-force blocking** | ✅ | ✅ | ✅ |
| **SSH guard** — bans SSH attackers from SSH alone, root included | ✅ | ✅ | ✅ |
| SELinux confinement (enforcing) | ✅ | ✅ | ✅ |
| Mail · DNS · MariaDB · FTPS/SFTP · Free SSL · Local backups | ✅ | ✅ | ✅ |
| Per-domain WAF rules, exceptions, trusted IPs | — | ✅ | ✅ |
| Speed Optimizer — dynamic page cache + CSS/JS minification | — | ✅ | ✅ |
| Commercial SSL upload · custom firewall port rules | — | ✅ | ✅ |
| Remote backups (S3-compatible · SFTP) | — | ✅ | ✅ |
| REST / JSON-RPC API | — | ✅ | ✅ |
| Admin + end-user views · client portal · per-user limits | — | — | ✅ |
| **Resellers** — own admins, own accounts, own ceilings | — | — | ✅ |
| WHMCS integration (native module + WHM-compatible API) | — | — | ✅ |
| Network protection — DDoS L7, Geo blocking, custom WAF rules | — | — | 🔜 Soon |
| Support | Docs | Standard | Priority |

The WAF families are **blocking on the free edition**. Not "log only", not "core rules".  
We refuse to sell you security that was already written.

---

PRICING: FLAT, PER SERVER
-------------------------

| Edition | Price (USD, excl. taxes) | What it's for |
| --- | --- | --- |
| **Personal** | Free | Developers, single-server owners — up to 20 sites |
| **Pro** | $14.90/mo or $149/yr per server | Managed hosting, high-traffic sites |
| **Business** | $24.99/mo or $249/yr per server | Hosting providers, agencies, resellers |

All prices are in USD, per server, billed monthly or yearly. Taxes (VAT/GST) are added at checkout where applicable

**Per server. Not per account.** Put 500 accounts on a Business box and the invoice doesn't  
move. A large part of the world pays less than the figures above — the checkout prices by country.

**14-day Pro or Business trial, no card**, offered at your first login. Install first, pay  
second: a license binds to the server's address, so there's nothing to buy before you've seen it run.

Paying from LatAm, Africa or South/Southeast Asia? Checkout will probably show you a friendlier number.

---

REQUIREMENTS
------------

* RHEL, AlmaLinux or Rocky **8, 9 or 10** — x86\_64, root.
* 2 GB RAM runs it; give it more if you're running mail + DNS + a real site (aren't we all).
* **SELinux enforcing.** Yes, on purpose.

---

🤝 LIMITATIONS
-------------

It only runs on RHEL-family systems (Ubuntu is on the roadmap, no date yet, no promises).

The panel is not open source. It's a young product, so bug reports get read and answered quickly by our support team.

I'll stay around to answer questions. Tear it apart. 🙂

---

FAQ
---

**Is the free edition crippled?**  
No. 20 sites is the only cap. Full blocking WAF, firewall, brute-force blocking, SSH guard,  
mail, DNS, SSL, backups — all in.

**Debian/Ubuntu?**  
Not yet. RHEL-family only today; the Ubuntu port is planned and not promised.

**Is this a skin over nginx/Apache/OLS?**  
No. CoreHttpd is ours, one static binary, `.htaccess`-compatible, WAF in-process.

**Do I need a license server / phone home?**  
Free edition: nothing to activate. Paid: the license binds to the server's public IP.

**Can I resell it?**  
Business. Each reseller gets their own administrators, their own accounts and their own ceilings, and sees neither the server nor their neighbours. WHMCS provisions it, both through our native module and through a WHM-compatible API for people with existing WHM integrations.

**What if I hate it?**  
If you transformed a cPanel box: roll back quickly, cPanel comes back whole. If it's a fresh install:  
it's a VPS, you know what to do. Either way, tell us here what made you hate it — that's worth  
more to us than the sale.

---

LINKS
-----

* 🏠 **[https://www.corepanel.net](https://www.corepanel.net?utm_source=lowendtalk "https://www.corepanel.net")**
* 🎛️ **Live demo:** [https://demo.corepanel.net](https://demo.corepanel.net?utm_source=lowendtalk "https://demo.corepanel.net")
* 📚 **Docs:** [https://www.corepanel.net/docs](https://www.corepanel.net/docs?utm_source=lowendtalk "https://www.corepanel.net/docs")
* 💬 **Questions:** right here in this thread, or PM me.

We're a small team and we built the whole thing — the panel, the web server, the WAF, the  
migration tool. Throw your worst at it.

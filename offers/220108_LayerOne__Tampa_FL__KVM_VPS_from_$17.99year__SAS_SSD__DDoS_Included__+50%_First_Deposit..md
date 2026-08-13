---
id: 220108
title: "LayerOne | Tampa FL | KVM VPS from $17.99/year | SAS SSD | DDoS Included | +50% First Deposit."
date: "2026-08-13T05:11:56+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/220108/layerone-tampa-fl-kvm-vps-from-17-99-year-sas-ssd-ddos-included-50-first-deposit"
---
# LayerOne | Tampa FL | KVM VPS from $17.99/year | SAS SSD | DDoS Included | +50% First Deposit.
**Link:** [Original Thread](https://lowendtalk.com/discussion/220108/layerone-tampa-fl-kvm-vps-from-17-99-year-sas-ssd-ddos-included-50-first-deposit)

Hello LET 👋

Quick overview of LayerOne:

We run KVM VPS out of Tampa, Florida on Intel Xeon Skylake-SP or better with SAS SSD  
storage, on hardware we own and colocate ourselves.

The part that makes us slightly different from most providers in this price range is  
billing. Everything runs from account credit, metered by the hour, so you can delete a  
server and stop paying for it that same hour rather than waiting out a term you already  
committed to. Yearly pricing is still there if you would rather prepay and forget about  
it.

Real prices, real specs, and I will answer anything in this thread including the  
uncomfortable questions.

**Offer page: <https://layeronecloud.com/let-promo/>**

---

⚡ THE OFFER
-----------

Two plans, both on the same platform as our standard range. No offer-tier hardware and  
no stripped features.

| Plan | vCPU | RAM | Disk | Transfer | Port | IPv4 | DDoS | Yearly | Hourly |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **Nano** | 1 | 1024 MB | 20 GB SAS SSD | 1 TB | 1 Gbps | ✅ 1 dedicated | ✅ | **$17.99** | $0.0034/hr |
| **Starter** | 1 | 2048 MB | 40 GB SAS SSD | 2 TB | 1 Gbps | ✅ 1 dedicated | ✅ | **$23.99** | $0.0047/hr |

Public prices are $28.80 and $48.00 a year, so that is 37% off Nano and 50% off  
Starter.

**Yearly** works out to roughly $1.50 and $2.00 a month.

**Hourly** works out to roughly $2.48 and $3.43 for a 730 hour month, against public  
rates of $3.00 and $5.00. A 31 day month bills a few hours more, because it is a few  
hours longer.

Offer notes:

* Stock is limited and the offer runs while it lasts.
* Hourly and yearly are the same plan at the same spec, just a different term.
* You can order more than one.
* Need larger? Our standard plans run up to 8 vCPU and 32 GB.

**On the network:** we our own ASN - AS31916 and take transit from four  
carriers, Hurricane Electric, GTT, NTT America and Arelion. That means no single  
upstream can take us offline on its own.

**On IPv6:** not available yet. It is a limitation on our upstream that is actively being worked on. If IPv6 is a requirement for what you are building, wait for us rather than ordering and being annoyed.

**IPV4:**: You can purchase floating IPs and delete, move, or purchase them at any time. The IP address assigned to your server cannot be modified.

---

🎁 50% FIRST DEPOSIT MATCH
-------------------------

Code: **`LOWENDTALK`**

We add 50% to your first deposit, up to $25 of bonus credit.

* Deposit $50, start with $75. That is the largest bonus available.
* Works from $5 upwards, matched at the same 50%.

---

🧾 HOW BILLING WORKS
-------------------

Worth thirty seconds if you have not used a credit based host before.

**1. Add credit.** Pay by card or crypto and the amount lands on your account as  
credit, plus the 50% match if it is your first deposit. Ordering a plan does both in  
one step.

**2. Deploy.** Pick a plan and an image and the server is built for you. Full root  
access, browser VNC console, and start, stop and rebuild from the client area.

**3. Draw down.** Each running hour meters against your credit at the rate for your  
plan and term. Yearly buys a year at the yearly rate. Delete the server and the  
metering stops.

If your balance gets low we email you before anything stops. If you have a card saved  
we top up automatically. Nothing is deleted without warning first.

---

✅ WHAT IS INCLUDED
------------------

| Feature | Nano | Starter |
| --- | --- | --- |
| Full root on KVM | ✅ | ✅ |
| Browser VNC console | ✅ | ✅ |
| Dedicated IPv4 | ✅ 1 | ✅ 1 |
| Always-on L3/L4 DDoS mitigation | ✅ | ✅ |
| SAS SSD storage | ✅ | ✅ |
| Start, stop, rebuild from client area | ✅ | ✅ |
| Daily snapshots, 7 day retention | Optional | Optional |
| Extra IPv4 addresses | Add-on | Add-on |

* **DDoS filtering** is on by default at no extra cost. Nothing to enable, no scrubbing  
  surcharge, no separate protected IP to order. Mitigation is provided by our upstream,  
  with our own filtering rules on top of it.
* **Snapshots** are switched on per server and billed hourly only while enabled.
* **Extra IPv4** addresses are billed hourly while reserved.

---

🎯 SET YOUR EXPECTATIONS
-----------------------

These are entry level plans at entry level prices, and I would rather say this here than  
in a refund thread.

* CPU is shared. We allocate with conservative oversubscription and we do not sell  
  denser than our capacity planning allows, but it is shared, and fair use applies.
* We are a small operation. Support is tickets answered by us, not a 24/7 NOC. We aim for a one day reply time but we do not provide an SLA on ticket responses, we only provide an SLA on critical level issues at our infrastructure. Application issues are best effort.
* Keep external backups of anything you care about. Snapshots are a convenience, not a  
  disaster recovery plan, and that is true at every provider regardless of what the  
  marketing says.
* No provider can promise that no attack ever gets through. Our filtering is always on  
  and handles the common volumetric cases. It is not magic.
* If you are unsure whether your workload fits, ask before you order rather than after.

What we do commit to: the price you buy at is the price you keep, we will tell you what  
actually broke when something breaks, and we will not pretend a four hour outage was  
five minutes.

One housekeeping note while we are being straightforward. This is our first offer under  
the LayerOne name. Some of you will have bought from us as Pulsar67. New hardware, new colocation facility, same staff.

---

🛠️ TECHNICAL INFORMATION
------------------------

|  |  |
| --- | --- |
| Virtualization | KVM |
| CPU | Intel Xeon Skylake-SP or better |
| Storage | SAS SSD |
| Hardware | Owned by us, colocated |
| Location | Tampa, Florida |
| Datacenter | WOW! Tampa colocation |
| ASN | AS31916, our own |
| Upstreams | Hurricane Electric, GTT Communications, NTT America, Arelion |
| Network | Dedicated IPv4. IPv6 pending upstream. |
| DDoS mitigation | Always-on L3/L4 upstream filtering, plus our own rules |
| Payments | Card and cryptocurrency |
| Test IPv4 | `207.174.22.1` |
| Status page | <https://layeronecloud.com/status/> |
| Client area | <https://layeronecloud.com/client> |
| Support | [[email protected]](/cdn-cgi/l/email-protection), or tickets from the client area |
| Legal | Terms of Service, SLA, Acceptable Use and Privacy Policy are all linked in the footer of <https://layeronecloud.com> |

Ping or MTR the test IP before you buy.
---------------------------------------

❓ QUESTIONS WORTH ASKING
------------------------

**Will this price go up on me later?**  
No. This offer is its own set of plans, and a server keeps the price of the plan it was  
bought on. When we change or end the offer we do it by publishing new plans, not by  
editing the ones people are already running. We may adjust plans as new hardware comes in, but we will continue to support your server at the same price while the hardware is the same.

**What happens when my yearly credit runs out?**  
If you have a card saved we top the balance up automatically. If you do not, we email  
you as the balance gets low so you can add credit before anything stops. Nothing is  
deleted without warning.

**Is the monthly option a contract?**  
No. Monthly is just our hourly billing at the offer rate, so you pay for the hours the  
server actually runs. Stop or delete it whenever you like and the metering stops with  
it. Unused credit stays on your account.

**Can I order more than one?**  
Yes. The credit match is once per customer rather than once per server, so deposit once  
and deploy as many of the offer plans as your credit covers.

**What can I run on it?**  
It is a KVM VPS with full root, so anything legal that fits in the plan. No  
cryptomining, no attack traffic, no spam. If you are unsure whether a workload fits,  
ask us before you order rather than after.

**How do I reach support?**  
Tickets from the client area, and we answer them ourselves. There is a contact form if  
you want to ask something before you have an account.

---

📦 ORDER
-------

**<https://layeronecloud.com/let-promo/>**

Deposit code: **`LOWENDTALK`** for the 50% first deposit match.

Questions in thread are welcome, including the skeptical ones. Bug reports and  
constructive feedback on the panel are welcome too. We would rather hear it than not.

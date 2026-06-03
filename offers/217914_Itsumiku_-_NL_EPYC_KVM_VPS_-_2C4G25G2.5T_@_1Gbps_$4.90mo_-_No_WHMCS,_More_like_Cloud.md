---
id: 217914
title: "Itsumiku - NL EPYC KVM VPS - 2C4G/25G/2.5T @ 1Gbps $4.90/mo - No WHMCS, More like Cloud"
date: "2026-06-03T18:44:11+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/217914/itsumiku-nl-epyc-kvm-vps-2c4g-25g-2-5t-1gbps-4-90-mo-no-whmcs-more-like-cloud"
---
# Itsumiku - NL EPYC KVM VPS - 2C4G/25G/2.5T @ 1Gbps $4.90/mo - No WHMCS, More like Cloud
**Link:** [Original Thread](https://lowendtalk.com/discussion/217914/itsumiku-nl-epyc-kvm-vps-2c4g-25g-2-5t-1gbps-4-90-mo-no-whmcs-more-like-cloud)

Hello LowEndTalk,

We are Itsumiku LLC, a new cloud hosting provider registered early 2026 in Wyoming, US. Launching our first VPS location in Naaldwijk, Netherlands.  
Itsumiku is also an ARIN member with AS402428.

This opening offer is for LET members: 30% off all Naaldwijk VPS plans, a traffic pack if you reply in this thread after ordering, and 3 free snapshot as add-ons.

We are new, so we are keeping billing simple and low-risk: monthly and quarterly only. No annual lock-in for this launch.

Why Itsumiku?
-------------

Itsumiku is our attempt to bring a more cloud-native product experience to the budget VPS market.

Many low-cost VPS offers stop at the same formula: CPU, RAM, disk, bandwidth. That is useful, but it does not leave much room for a platform to grow.

Our approach is different. We do not use a simple WHMCS connected to a VPS panel. We have developed our own platform covering from billing to virtualization. The first public product is simple KVM VPS, but the platform is designed to support more than fixed-size virtual servers.

For this LET launch, that means:

* Fast EPYC CPU (EPYC 7402P), DDR4 Memory, Micron Enterprise NVMe Disk
* Transparent VPS plans with clear monthly pricing
* Shared traffic pools: included transfer from each VPS is added to your account pool, and all your VMs draw from it together
* EU/US pool roadmap: as more Itsumiku regions launch, European and North American regions are planned to share one traffic pool
* Optional traffic packs for users who outgrow the combined transfer included with their VMs
* Every VM includes 1 free snapshot slot and use coupon code to get 2 additional FREE snapshots

We know LET users care about price, but we also know many of you care about whether a provider is building something sustainable. This launch is our first public step in that direction.

Location
--------

Current:

* Naaldwijk, Netherlands

Opening Sale Plans
------------------

Use promo code `X65N9LGHH0TH` to get a 30% recurring discount. Valid until 21st June.

| Plan | vCPU | RAM | Disk | Traffic | Port | LET Price |
| --- | --- | --- | --- | --- | --- | --- |
| EPYC-1C1G | 1 vCore | 1 GiB | 10 GiB | 1.0 TiB | 1Gbps | $1.58/mo or $4.52/qtr |
| EPYC-1C2G | 1 vCore | 2 GiB | 15 GiB | 1.5 TiB | 1Gbps | $2.77/mo or $7.88/qtr |
| EPYC-2C4G | 2 vCores | 4 GiB | 25 GiB | 2.5 TiB | 1Gbps | $4.90/mo or $13.97/qtr |
| EPYC-4C8G | 4 vCores | 8 GiB | 40 GiB | 4.0 TiB | 1Gbps | $8.93/mo or $25.41/qtr |

Original monthly prices are $2.25, $3.95, $7.00, and $12.75.  
Order Here: <https://portal.itsumiku.com>

LET Reply Bonus
---------------

The data package is valid for life, until it is used up. And monthly quota included in VM will be used first.  
Reply in this thread with your invoice number after purchase and we will add a free traffic pack:

* EPYC-1C1G / EPYC-1C2G: +512 GiB
* EPYC-2C4G: +1 TiB
* EPYC-4C8G: +2 TiB

This is bonus traffic pack added to your account traffic pool, not a permanent monthly quota change.

Snapshot Coupon
---------------

Every VM already includes 1 free snapshot.

For this launch, you can also use coupon code `TIUW5XD71EUN` to get 2 additional snapshots for free for a limited time. Valid until 21st June.

That gives you 3 snapshot slots in total:

* 1 included snapshot
* 2 free snapshot with coupon `TIUW5XD71EUN`

Feedback / Bug Hunt
-------------------

We are also inviting LET users to try the platform seriously and tell us what feels wrong, confusing, or broken.

If you find an undiscovered bug, an awkward ordering flow, unclear traffic pool behavior, confusing panel text, or anything that should be improved, please post it in this thread or open a ticket. We are especially interested in feedback on:

* Ordering and checkout
* VPS lifecycle actions
* Snapshot add-ons
* Traffic pool
* Traffic pack
* Panel wording and UX
* Network performance

Good For
--------

* Small or medium websites
* Dev environment
* Personal projects
* VPN / proxy within AUP
* Users who want a budget VPS backed by a more structured cloud platform
* And many more!

Test / Network
--------------

Test IPv4: 157.254.131.9  
Test IPv6: 2a00:7c80:0:4a::9  
YABS:

```
Tue Jun  2 11:06:01 AM UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 0 minutes
Processor  : AMD EPYC-Rome-v5 Processor
CPU cores  : 2 @ 2794.750 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ❌ Disabled
RAM        : 3.8 GiB
Swap       : 0.0 KiB
Disk       : 24.5 GiB
Distro     : Debian GNU/Linux 13 (trixie)
Kernel     : 6.12.90+deb13.1-amd64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : WorldStream B.V.
ASN        : AS49981 WorldStream B.V.
Host       : WorldStream B.V.
Location   : Naaldwijk, South Holland (ZH)
Country    : Netherlands

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/sda3):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 275.83 MB/s  (68.9k) | 2.17 GB/s    (33.9k)
Write      | 276.55 MB/s  (69.1k) | 2.18 GB/s    (34.1k)
Total      | 552.39 MB/s (138.0k) | 4.35 GB/s    (68.0k)
           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 5.49 GB/s    (10.7k) | 5.50 GB/s     (5.3k)
Write      | 5.78 GB/s    (11.2k) | 5.86 GB/s     (5.7k)
Total      | 11.27 GB/s   (22.0k) | 11.36 GB/s   (11.0k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 938 Mbits/sec   | busy            | 8.72 ms        
Eranium         | Amsterdam, NL (100G)      | 941 Mbits/sec   | 941 Mbits/sec   | 1.37 ms        
Uztelecom       | Tashkent, UZ (10G)        | 870 Mbits/sec   | 891 Mbits/sec   | 96.0 ms        
Leaseweb        | Singapore, SG (10G)       | 783 Mbits/sec   | 846 Mbits/sec   | 159 ms         
Clouvider       | Los Angeles, CA, US (10G) | 748 Mbits/sec   | 855 Mbits/sec   | 140 ms         
Leaseweb        | NYC, NY, US (10G)         | 854 Mbits/sec   | 901 Mbits/sec   | 75.8 ms        
Edgoo           | Sao Paulo, BR (1G)        | 689 Mbits/sec   | 824 Mbits/sec   | 182 ms         

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 925 Mbits/sec   | 926 Mbits/sec   | 8.63 ms        
Eranium         | Amsterdam, NL (100G)      | 928 Mbits/sec   | 928 Mbits/sec   | 1.36 ms        
Uztelecom       | Tashkent, UZ (10G)        | 862 Mbits/sec   | 874 Mbits/sec   | 95.8 ms        
Leaseweb        | Singapore, SG (10G)       | 781 Mbits/sec   | 833 Mbits/sec   | 160 ms         
Clouvider       | Los Angeles, CA, US (10G) | 739 Mbits/sec   | 843 Mbits/sec   | 140 ms         
Leaseweb        | NYC, NY, US (10G)         | 822 Mbits/sec   | 891 Mbits/sec   | --             
Edgoo           | Sao Paulo, BR (1G)        | 737 Mbits/sec   | 811 Mbits/sec   | 182 ms         

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value                         
                |                               
Single Core     | 1403
Multi Core      | 2569
Full Test       | https://browser.geekbench.com/v6/cpu/18210163

YABS completed in 15 min 16 sec
```

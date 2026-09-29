---
id: 221558
title: "D4 Networks | 4GB KVM, 80-120GB NVMe | $49/year, renews at $49 | Dallas, Amsterdam, New York"
date: "2026-09-28T18:46:54+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/221558/d4-networks-4gb-kvm-80-120gb-nvme-49-year-renews-at-49-dallas-amsterdam-new-york"
---
# D4 Networks | 4GB KVM, 80-120GB NVMe | $49/year, renews at $49 | Dallas, Amsterdam, New York
**Link:** [Original Thread](https://lowendtalk.com/discussion/221558/d4-networks-4gb-kvm-80-120gb-nvme-49-year-renews-at-49-dallas-amsterdam-new-york)

Hello LET. First offer thread from us.

We're D4 Networks L.L.C., a Missouri company since 2014. Our ASN and IP space are our own, both from ARIN since 2015 (AS14475). More about us at the bottom.

**The special: 2 vCPU, 4 GB RAM, 80 to 120 GB NVMe and 5 TB monthly transfer for $49 per year, renewing at $49 per year.** Dedicated IPv4 and a routed /64 IPv6, in Dallas, Amsterdam and New York. Annual billing only. The price is locked until you cancel or move to another plan ([terms, section 4](https://d4networks.com/terms#t4)). All prices USD.

### Dallas: $49 per year

* 2 vCPU (shared), 4 GB RAM, 120 GB NVMe
* 5 TB monthly transfer, 4 Gbps port
* Disk: 10,000 IOPS / 300 MB/s, reads and writes combined
* Dedicated IPv4 + routed /64 IPv6, DDoS protection included
* Host: AMD EPYC 7543P, Micron 7450 PRO NVMe
* Downtown Dallas, fiber to the Equinix carrier hotel
* Limited to 40 units
* [Order Dallas, $49/year](https://my.d4networks.com/index.php?rp=/store/let-special/dallas-let-special)

### Amsterdam: $49 per year

* 2 vCPU (shared), 4 GB RAM, 80 GB NVMe
* 5 TB monthly transfer, 2.5 Gbps port
* Disk: 10,000 IOPS / 300 MB/s, reads and writes combined
* Dedicated IPv4 + routed /64 IPv6, DDoS protection included
* Host: AMD EPYC 7C13, Micron 7450 NVMe
* Digital Realty AMS17, Science Park
* Limited to 15 units
* [Order Amsterdam, $49/year](https://my.d4networks.com/index.php?rp=/store/let-special/amsterdam-let-special)

### New York: $49 per year

* 2 vCPU (shared), 4 GB RAM, 80 GB NVMe
* 5 TB monthly transfer, 2.5 Gbps port
* Disk: 10,000 IOPS / 300 MB/s, reads and writes combined
* Dedicated IPv4 + routed /64 IPv6, DDoS protection included
* Host: dual Intel Xeon Gold 6138, Kioxia CD6-R NVMe
* Telehouse, Staten Island
* Limited to 15 units
* [Order New York, $49/year](https://my.d4networks.com/index.php?rp=/store/let-special/nyc-let-special)

### Geekbench 6

One run per location; the full YABS output is at the bottom.

* Dallas: [1758 single / 3189 multi](https://browser.geekbench.com/v6/cpu/19268021)
* Amsterdam: [1731 single / 3106 multi](https://browser.geekbench.com/v6/cpu/19268020)
* New York: [1148 single / 2036 multi](https://browser.geekbench.com/v6/cpu/19268025)

New York runs on older Xeon Gold hosts and the scores show it. Same price; you are buying the New York location and routes. If CPU matters most, take Dallas.

### How the limits work

* Disk I/O is capped per VM at 10,000 IOPS and 300 MB/s, with reads and writes counted together. These are maximums, not guaranteed speeds.
* vCPUs are shared. Steady heavy CPU use that slows other customers down may be throttled ([terms, section 9](https://d4networks.com/terms#t9)).
* Port speeds are per-VM limits on a shared uplink.
* Transfer is counted outbound only and resets monthly, annual plans included. At the allowance the port drops to 10 Mbps until the reset, and you get an email before that happens. No overage bills, and we never power a VM off over bandwidth. Extra transfer is $2 per TB, open a ticket.

### Included

* Full root access (unmanaged)
* SolusVM 2 panel; deploys in about a minute once payment clears and the fraud check passes
* Custom ISOs by URL from the panel
* 1 snapshot + 1 backup slot (both started by you; the backup is copied to our remote storage)
* Private networking between your VMs in the same region
* rDNS
* 99.9% uptime SLA with service credits
* 24/7 ticket support

### Terms

* Annual billing only. Renews at $49 per year until you cancel or move to another plan.
* Upgrades move the service to a public plan at that plan's price. The $49 lock does not carry over.
* No extra IPv4 on the specials.
* Refunds: request within 24 hours of purchase.
* Cancel any time from the client area.
* Payments: Stripe (cards), PayPal, crypto (BTC and USDT). No tax added.

Prefer monthly billing? Our regular VPS plans start at $6 per month: [d4networks.com/cloud-vps](https://d4networks.com/cloud-vps)

### Policies

* VPN: allowed. Personal or commercial, lawful use.
* Outbound mail ports (25, 465, 587) are blocked by default. Open a ticket with a one-line description of your mail use and we open them, usually the same day.
* Torrents: legal content P2P is allowed within your transfer allowance.
* Abuse and DMCA complaints: you get a notice and 24 hours to respond before suspension. Active attacks, spam runs and legal orders can be suspended right away ([AUP, section 10](https://d4networks.com/acceptable-use#a10)).
* Tor: relays and bridges are fine. Exit nodes need prior approval.
* Mining: not permitted on any service. A service used for mining is terminated without refund.
* Fraud screening: orders are fraud-scored. Flagged orders get a human review, not a silent cancel. Ordering over a VPN is not an automatic reject.

### Test before you buy

[Looking glass](https://d4networks.com/looking-glass): ping, traceroute and mtr from every location. Geofeed (RFC 8805): [geofeed.d4networks.com](https://geofeed.d4networks.com/)

Test IPs:

* Dallas: 66.85.92.4 and 2602:f38e:1:1::1
* Amsterdam: 66.85.95.6 and 2602:f38e:4:1::1
* New York: 66.85.94.48 and 2602:f38e:2:1::1

Network: our upstream providers at each site carry transit from Cogent, GTT, Hurricane Electric, Lumen and Arelion (mix varies by site) and connect to Equinix IX, NYIIX and AMS-IX.

### About D4

D4 Networks L.L.C. has been on the Missouri register since November 24, 2014 (charter LC001426346). ARIN assigned us AS14475 in January 2015 and our /22 (66.85.92.0/22) in March 2015. The network moved onto its current upstreams earlier this year. Status page with 30 day history: [status.d4networks.com](https://status.d4networks.com)

[Terms](https://d4networks.com/terms) | [Acceptable use](https://d4networks.com/acceptable-use) | [SLA](https://d4networks.com/terms#t12)

### Benchmarks, September 28, 2026

One YABS run per location, each on a VM of the special above. Results vary with workload, host activity and destination.

The disk lines in the YABS cap at the plan limit. That is expected, the caps are enforced. YABS runs a 50/50 read/write mix, so read and write each show about half and the Total row shows the cap, which is why the disk numbers match in all three locations. The Geekbench score fields are blank because YABS can't read scores back from Geekbench's site at the moment (known YABS issue, fixed once Geekbench 6.7.2 ships). The runs uploaded fine; the scores are linked above.

Dallas:

```
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-09-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Mon Sep 28 09:41:05 AM UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 1 minutes
Processor  : AMD EPYC 7543P 32-Core Processor
CPU cores  : 2 @ 2794.748 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 3.8 GiB
Swap       : 0.0 KiB
Disk       : 119.9 GiB
Distro     : AlmaLinux 10.2 (Lavender Lion)
Kernel     : 6.12.0-211.47.1.el10_2.x86_64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : D4 Networks L.L.C.
ASN        : AS14475 D4 Networks L.L.C.
Host       : D4 Networks L.L.C. - Dallas
Location   : Dallas, Texas (TX)
Country    : United States

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/vda4):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 20.53 MB/s    (5.0k) | 150.65 MB/s   (2.2k)
Write      | 20.55 MB/s    (5.0k) | 151.44 MB/s   (2.3k)
Total      | 41.08 MB/s   (10.0k) | 302.10 MB/s   (4.6k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 147.15 MB/s    (280) | 146.20 MB/s    (139)
Write      | 154.97 MB/s    (295) | 155.94 MB/s    (148)
Total      | 302.12 MB/s    (575) | 302.14 MB/s    (287)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 1.32 Gbits/sec  | 1.53 Gbits/sec  | 108 ms
Eranium         | Amsterdam, NL (100G)      | 1.90 Gbits/sec  | 2.12 Gbits/sec  | 112 ms
Uztelecom       | Tashkent, UZ (10G)        | 1.01 Gbits/sec  | busy            | 202 ms
Leaseweb        | Singapore, SG (10G)       | 923 Mbits/sec   | 1.14 Gbits/sec  | 192 ms
Clouvider       | Los Angeles, CA, US (10G) | 2.59 Gbits/sec  | 3.10 Gbits/sec  | 38.0 ms
Leaseweb        | NYC, NY, US (10G)         | 3.83 Gbits/sec  | 3.63 Gbits/sec  | 37.6 ms
Edgoo           | Sao Paulo, BR (1G)        | 1.53 Gbits/sec  | 1.65 Gbits/sec  | 133 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 1.64 Gbits/sec  | 1.98 Gbits/sec  | 108 ms
Eranium         | Amsterdam, NL (100G)      | 1.99 Gbits/sec  | 2.17 Gbits/sec  | 113 ms
Uztelecom       | Tashkent, UZ (10G)        | busy            | 534 Mbits/sec   | --
Leaseweb        | Singapore, SG (10G)       | 740 Mbits/sec   | 979 Mbits/sec   | 224 ms
Clouvider       | Los Angeles, CA, US (10G) | 1.83 Gbits/sec  | 3.65 Gbits/sec  | 37.7 ms
Leaseweb        | NYC, NY, US (10G)         | 3.54 Gbits/sec  | 3.64 Gbits/sec  | 37.5 ms
Edgoo           | Sao Paulo, BR (1G)        | 1.48 Gbits/sec  | 1.48 Gbits/sec  | 137 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     |
Multi Core      |
Full Test       | https://browser.geekbench.com/v6/cpu/19268021

YABS completed in 14 min 50 sec
```

Amsterdam:

```
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-09-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Mon Sep 28 09:41:08 AM UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 2 minutes
Processor  : AMD EPYC 7C13 64-Core Processor
CPU cores  : 2 @ 1999.999 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 3.8 GiB
Swap       : 0.0 KiB
Disk       : 79.9 GiB
Distro     : AlmaLinux 10.2 (Lavender Lion)
Kernel     : 6.12.0-211.47.1.el10_2.x86_64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : D4 Networks L.L.C.
ASN        : AS14475 D4 Networks L.L.C.
Host       : D4 Networks L.L.C.
Location   : Amsterdam, North Holland (NH)
Country    : The Netherlands

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/vda4):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 20.53 MB/s    (5.0k) | 150.65 MB/s   (2.2k)
Write      | 20.54 MB/s    (5.0k) | 151.44 MB/s   (2.3k)
Total      | 41.08 MB/s   (10.0k) | 302.10 MB/s   (4.6k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 147.15 MB/s    (280) | 146.20 MB/s    (139)
Write      | 154.97 MB/s    (295) | 155.94 MB/s    (148)
Total      | 302.12 MB/s    (575) | 302.14 MB/s    (287)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 2.25 Gbits/sec  | 1.92 Gbits/sec  | 6.94 ms
Eranium         | Amsterdam, NL (100G)      | 2.50 Gbits/sec  | 2.37 Gbits/sec  | 0.320 ms
Uztelecom       | Tashkent, UZ (10G)        | 2.31 Gbits/sec  | 1.72 Gbits/sec  | 90.9 ms
Leaseweb        | Singapore, SG (10G)       | 881 Mbits/sec   | 1.40 Gbits/sec  | 162 ms
Clouvider       | Los Angeles, CA, US (10G) | 482 Mbits/sec   | 1.69 Gbits/sec  | 130 ms
Leaseweb        | NYC, NY, US (10G)         | 1.89 Gbits/sec  | 2.20 Gbits/sec  | 76.3 ms
Edgoo           | Sao Paulo, BR (1G)        | 979 Mbits/sec   | 1.22 Gbits/sec  | 182 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 2.46 Gbits/sec  | 2.33 Gbits/sec  | 6.99 ms
Eranium         | Amsterdam, NL (100G)      | 2.50 Gbits/sec  | 2.33 Gbits/sec  | 0.778 ms
Uztelecom       | Tashkent, UZ (10G)        | 2.11 Gbits/sec  | 1.61 Gbits/sec  | 94.3 ms
Leaseweb        | Singapore, SG (10G)       | 886 Mbits/sec   | 874 Mbits/sec   | --
Clouvider       | Los Angeles, CA, US (10G) | 857 Mbits/sec   | 1.50 Gbits/sec  | 144 ms
Leaseweb        | NYC, NY, US (10G)         | 2.13 Gbits/sec  | 2.20 Gbits/sec  | 75.4 ms
Edgoo           | Sao Paulo, BR (1G)        | 1.07 Gbits/sec  | 1.17 Gbits/sec  | 183 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     |
Multi Core      |
Full Test       | https://browser.geekbench.com/v6/cpu/19268020

YABS completed in 14 min 16 sec
```

New York:

```
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-09-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Mon Sep 28 09:41:01 AM UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 1 minutes
Processor  : Intel(R) Xeon(R) Gold 6138 CPU @ 2.00GHz
CPU cores  : 2 @ 2000.000 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 3.8 GiB
Swap       : 0.0 KiB
Disk       : 79.9 GiB
Distro     : AlmaLinux 10.2 (Lavender Lion)
Kernel     : 6.12.0-211.47.1.el10_2.x86_64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : D4 Networks L.L.C.
ASN        : AS14475 D4 Networks L.L.C.
Host       : D4 Networks L.L.C. - New York
Location   : Staten Island, New York (NY)
Country    : United States

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/vda4):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 20.54 MB/s    (5.0k) | 150.65 MB/s   (2.2k)
Write      | 20.55 MB/s    (5.0k) | 151.44 MB/s   (2.3k)
Total      | 41.09 MB/s   (10.0k) | 302.10 MB/s   (4.6k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 147.16 MB/s    (280) | 146.20 MB/s    (139)
Write      | 154.98 MB/s    (295) | 155.94 MB/s    (148)
Total      | 302.14 MB/s    (575) | 302.14 MB/s    (287)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 1.85 Gbits/sec  | 1.96 Gbits/sec  | 71.4 ms
Eranium         | Amsterdam, NL (100G)      | 2.24 Gbits/sec  | 2.25 Gbits/sec  | 75.5 ms
Uztelecom       | Tashkent, UZ (10G)        | 24.2 Mbits/sec  | 892 Mbits/sec   | 230 ms
Leaseweb        | Singapore, SG (10G)       | 615 Mbits/sec   | 963 Mbits/sec   | 227 ms
Clouvider       | Los Angeles, CA, US (10G) | 1.04 Gbits/sec  | 2.27 Gbits/sec  | 80.1 ms
Leaseweb        | NYC, NY, US (10G)         | 2.51 Gbits/sec  | 2.37 Gbits/sec  | 2.27 ms
Edgoo           | Sao Paulo, BR (1G)        | 1.77 Gbits/sec  | 1.75 Gbits/sec  | 112 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 1.84 Gbits/sec  | 2.23 Gbits/sec  | 68.1 ms
Eranium         | Amsterdam, NL (100G)      | 2.36 Gbits/sec  | 2.22 Gbits/sec  | 72.1 ms
Uztelecom       | Tashkent, UZ (10G)        | 1.19 Gbits/sec  | 1.27 Gbits/sec  | 156 ms
Leaseweb        | Singapore, SG (10G)       | 532 Mbits/sec   | 953 Mbits/sec   | 225 ms
Clouvider       | Los Angeles, CA, US (10G) | 721 Mbits/sec   | 2.22 Gbits/sec  | 76.6 ms
Leaseweb        | NYC, NY, US (10G)         | 2.51 Gbits/sec  | 2.33 Gbits/sec  | 2.56 ms
Edgoo           | Sao Paulo, BR (1G)        | 1.90 Gbits/sec  | 2.15 Gbits/sec  | 111 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     |
Multi Core      |
Full Test       | https://browser.geekbench.com/v6/cpu/19268025

YABS completed in 15 min 59 sec
```

Questions welcome, we answer in the thread.

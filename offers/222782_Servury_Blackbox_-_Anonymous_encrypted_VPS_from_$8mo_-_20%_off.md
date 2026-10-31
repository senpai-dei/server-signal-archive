---
id: 222782
title: "Servury Blackbox - Anonymous encrypted VPS from $8/mo - 20% off"
date: "2026-10-31T07:19:58+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/222782/servury-blackbox-anonymous-encrypted-vps-from-8-mo-20-off"
---
# Servury Blackbox - Anonymous encrypted VPS from $8/mo - 20% off
**Link:** [Original Thread](https://lowendtalk.com/discussion/222782/servury-blackbox-anonymous-encrypted-vps-from-8-mo-20-off)

![](https://servury.com/assets/img/promo/banner.png)

---

Hello LET community,

Servury is an anonymous hosting service that doesn't require KYC or personal information.  
You can log in with your generated unique credential and access your encrypted server through your own dashboard or via SSH.

**Features:**  
- 8 global locations and multiple plans, with flexible billing cycles.  
- Zero logs  
- No Javascript  
- Human support

We don't inspect network packets, collect traffic logs, or monitor user activity. Since we don't retain this data, there's nothing to hand over.

We accept: Crypto, Cash, Cards

Use code **LET20** for a 20% discount!

Get your first server today : **<https://servury.com/>**

---

The server
==========

| Plan | CPU | RAM | Storage | Port | Bandwidth | Price |
| --- | --- | --- | --- | --- | --- | --- |
| Blackbox Core | 2x EPYC 7B13 (SEV-SNP) | 4 GB DDR4 | 50 GB NVMe | 10 Gbps | 4 TB / 31 days | $9.99 |

**All Blackbox plans include:**  
- Encrypted storage (LUKS2)  
- Encrypted RAM (SEV-SNP)  
- Measured boot  
- Custom ISO, UKI or disk image  
- Dedicated /64 IPv6 block  
- BYOIP  
- rDNS  
- Human-read abuse reports

YABS

```
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-07-24                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Fri Aug 21 01:49:49 AM UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 1 minutes
Processor  : AMD EPYC-v4 Processor
CPU cores  : 2 @ 2794.748 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ❌ Disabled
RAM        : 3.8 GiB
Swap       : 0.0 KiB
Disk       : 49.1 GiB
Distro     : Debian GNU/Linux 13 (trixie)
Kernel     : 6.12.101+deb13-amd64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : Servury
ASN        : AS395904 Servury
Host       : Servury
Location   : Montreal, Quebec (QC)
Country    : Canada

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/sda3):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 281.33 MB/s  (68.6k) | 3.68 GB/s    (56.1k)
Write      | 282.08 MB/s  (68.8k) | 3.69 GB/s    (56.4k)
Total      | 563.42 MB/s (137.5k) | 7.37 GB/s   (112.6k)
           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 12.83 GB/s   (24.4k) | 3.39 GB/s     (3.2k)
Write      | 13.51 GB/s   (25.7k) | 3.62 GB/s     (3.4k)
Total      | 26.34 GB/s   (50.2k) | 7.01 GB/s     (6.6k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           

Clouvider       | London, UK (10G)          | 2.31 Gbits/sec  | 3.11 Gbits/sec  | 71.6 ms        

Eranium         | Amsterdam, NL (100G)      | 2.70 Gbits/sec  | 3.02 Gbits/sec  | 79.7 ms        

Uztelecom       | Tashkent, UZ (10G)        | 1.08 Gbits/sec  | 1.12 Gbits/sec  | 169 ms         

Leaseweb        | Singapore, SG (10G)       | 643 Mbits/sec   | 900 Mbits/sec   | 246 ms         

Clouvider       | Los Angeles, CA, US (10G) | 3.28 Gbits/sec  | 3.83 Gbits/sec  | 57.8 ms        

Leaseweb        | NYC, NY, US (10G)         | 9.17 Gbits/sec  | 8.40 Gbits/sec  | 9.92 ms        

Edgoo           | Sao Paulo, BR (1G)        | 1.59 Gbits/sec  | 1.99 Gbits/sec  | 119 ms         

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           

Clouvider       | London, UK (10G)          | 2.64 Gbits/sec  | 3.03 Gbits/sec  | 70.6 ms        

Eranium         | Amsterdam, NL (100G)      | 2.63 Gbits/sec  | 3.06 Gbits/sec  | 80.3 ms        

Uztelecom       | Tashkent, UZ (10G)        | 1.04 Gbits/sec  | 1.26 Gbits/sec  | 169 ms         

Leaseweb        | Singapore, SG (10G)       | 694 Mbits/sec   | 905 Mbits/sec   | 239 ms         

Clouvider       | Los Angeles, CA, US (10G) | 3.26 Gbits/sec  | 3.92 Gbits/sec  | 57.8 ms        

Leaseweb        | NYC, NY, US (10G)         | 9.22 Gbits/sec  | 9.23 Gbits/sec  | 10.0 ms        

Edgoo           | Sao Paulo, BR (1G)        | 1.62 Gbits/sec  | 2.00 Gbits/sec  | 125 ms         

---------------------------------
Test            | Value                         
                |                               
Single Core     | 1809                          
Multi Core      | 3316                          
Full Test       | https://browser.geekbench.com/v6/cpu/19039180

YABS completed in 13 min 23 sec
```

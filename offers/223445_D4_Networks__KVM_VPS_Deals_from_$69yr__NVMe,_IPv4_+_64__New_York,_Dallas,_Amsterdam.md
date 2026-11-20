---
id: 223445
title: "D4 Networks | KVM VPS Deals from $69/yr | NVMe, IPv4 + /64 | New York, Dallas, Amsterdam"
date: "2026-11-18T23:37:12+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/223445/d4-networks-kvm-vps-deals-from-69-yr-nvme-ipv4-64-new-york-dallas-amsterdam"
---
# D4 Networks | KVM VPS Deals from $69/yr | NVMe, IPv4 + /64 | New York, Dallas, Amsterdam
**Link:** [Original Thread](https://lowendtalk.com/discussion/223445/d4-networks-kvm-vps-deals-from-69-yr-nvme-ipv4-64-new-york-dallas-amsterdam)

Hi LET,

Two KVM plans for the season, in New York, Dallas and Amsterdam. Same price every year you renew, no setup fee. Limited stock, the offer ends on Thanksgiving, November 26 at 11:59 PM PST, or when the units are gone.

**KVM 5 GB | $69 a year, renews at $69**

* 2 vCPU
* 5 GB RAM
* 100 GB NVMe
* 6 TB monthly transfer
* 1 dedicated IPv4 + routed /64 IPv6
* KVM, full root, custom ISO supported
* Double disk speed limits on these deals, 20,000 IOPS and 600 MB/s per VM
* Port speed 2.5 Gbps in New York and Amsterdam, 4 Gbps in Dallas
* DDoS protection included

Order New York <https://my.d4networks.com/cart.php?a=add&pid=73>  
Order Dallas <https://my.d4networks.com/cart.php?a=add&pid=74>  
Order Amsterdam <https://my.d4networks.com/cart.php?a=add&pid=75>

**KVM 7 GB | $89 a year, renews at $89**

* 3 vCPU
* 7 GB RAM
* 140 GB NVMe
* 8 TB monthly transfer
* 1 dedicated IPv4 + routed /64 IPv6
* KVM, full root, custom ISO supported
* Double disk speed limits on these deals, 20,000 IOPS and 600 MB/s per VM
* Port speed 2.5 Gbps in New York and Amsterdam, 4 Gbps in Dallas
* DDoS protection included

Order New York <https://my.d4networks.com/cart.php?a=add&pid=76>  
Order Dallas <https://my.d4networks.com/cart.php?a=add&pid=77>  
Order Amsterdam <https://my.d4networks.com/cart.php?a=add&pid=78>

**Bonus**

* Post your order number in this thread and we add a 13th month for free, so you get 13 months for the price of 12.

Pay by card, PayPal or crypto.

**Benchmarks**

YABS New York, KVM 7 GB (click to open)

```
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-10-31                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Tue Nov 17 12:58:56 PM UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 16 minutes
Processor  : Intel(R) Xeon(R) Gold 6138 CPU @ 2.00GHz
CPU cores  : 3 @ 2000.000 MHz
AES-NI     : ✔️ Enabled
VM-x/AMD-V : ✔️ Enabled
RAM        : 6.8 GiB
Swap       : 0.0 KiB
Disk       : 139.9 GiB
Distro     : AlmaLinux 10.2 (Lavender Lion)
Kernel     : 6.12.0-211.47.1.el10_2.x86_64
VM Type    : KVM
IPv4/IPv6  : ✔️ Online / ✔️ Online

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
Read       | 41.04 MB/s   (10.0k) | 303.42 MB/s   (4.6k)
Write      | 41.14 MB/s   (10.0k) | 305.01 MB/s   (4.6k)
Total      | 82.18 MB/s   (20.0k) | 608.43 MB/s   (9.2k)
           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 296.34 MB/s    (565) | 294.41 MB/s    (280)
Write      | 312.09 MB/s    (595) | 314.02 MB/s    (299)
Total      | 608.43 MB/s   (1.1k) | 608.43 MB/s    (579)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 1.98 Gbits/sec  | 2.21 Gbits/sec  | 71.6 ms        
Eranium         | Amsterdam, NL (100G)      | 2.24 Gbits/sec  | 2.23 Gbits/sec  | 75.1 ms        
Uztelecom       | Tashkent, UZ (10G)        | 363 Mbits/sec   | 756 Mbits/sec   | 242 ms         
Leaseweb        | Singapore, SG (10G)       | 654 Mbits/sec   | 980 Mbits/sec   | 218 ms         
Clouvider       | Los Angeles, CA, US (10G) | 1.93 Gbits/sec  | busy            | 63.0 ms        
Leaseweb        | NYC, NY, US (10G)         | 2.51 Gbits/sec  | 2.34 Gbits/sec  | 2.30 ms        
Edgoo           | Sao Paulo, BR (1G)        | busy            | busy            | 111 ms         

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 2.36 Gbits/sec  | busy            | 69.3 ms        
Eranium         | Amsterdam, NL (100G)      | 2.31 Gbits/sec  | 2.20 Gbits/sec  | 73.4 ms        
Uztelecom       | Tashkent, UZ (10G)        | 871 Mbits/sec   | 1.24 Gbits/sec  | 174 ms         
Leaseweb        | Singapore, SG (10G)       | busy            | 1.01 Gbits/sec  | 220 ms         
Clouvider       | Los Angeles, CA, US (10G) | 2.20 Gbits/sec  | 1.98 Gbits/sec  | 63.0 ms        
Leaseweb        | NYC, NY, US (10G)         | busy            | 2.31 Gbits/sec  | 2.32 ms        
Edgoo           | Sao Paulo, BR (1G)        | busy            | busy            | 111 ms         

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value                         
                |                               
Single Core     | 1071                          
Multi Core      | 2707                          
Full Test       | https://browser.geekbench.com/v6/cpu/19485157

YABS completed in 15 min 4 sec
```

YABS Dallas, KVM 7 GB (click to open)

```
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-10-31                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Tue Nov 17 12:58:58 PM UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 6 minutes
Processor  : AMD EPYC 7543P 32-Core Processor
CPU cores  : 3 @ 2794.748 MHz
AES-NI     : ✔️ Enabled
VM-x/AMD-V : ✔️ Enabled
RAM        : 6.8 GiB
Swap       : 0.0 KiB
Disk       : 139.9 GiB
Distro     : AlmaLinux 10.2 (Lavender Lion)
Kernel     : 6.12.0-211.47.1.el10_2.x86_64
VM Type    : KVM
IPv4/IPv6  : ✔️ Online / ✔️ Online

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
Read       | 41.04 MB/s   (10.0k) | 303.42 MB/s   (4.6k)
Write      | 41.14 MB/s   (10.0k) | 305.01 MB/s   (4.6k)
Total      | 82.18 MB/s   (20.0k) | 608.43 MB/s   (9.2k)
           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 296.59 MB/s    (565) | 294.41 MB/s    (280)
Write      | 312.35 MB/s    (595) | 314.02 MB/s    (299)
Total      | 608.95 MB/s   (1.1k) | 608.43 MB/s    (579)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 1.02 Gbits/sec  | 1.80 Gbits/sec  | 108 ms         
Eranium         | Amsterdam, NL (100G)      | 1.41 Gbits/sec  | 2.15 Gbits/sec  | 120 ms         
Uztelecom       | Tashkent, UZ (10G)        | 687 Mbits/sec   | 829 Mbits/sec   | 216 ms         
Leaseweb        | Singapore, SG (10G)       | 762 Mbits/sec   | 1.16 Gbits/sec  | 196 ms         
Clouvider       | Los Angeles, CA, US (10G) | 3.61 Gbits/sec  | 643 Mbits/sec   | 31.5 ms        
Leaseweb        | NYC, NY, US (10G)         | 3.86 Gbits/sec  | 3.54 Gbits/sec  | 37.3 ms        
Edgoo           | Sao Paulo, BR (1G)        | busy            | busy            | 133 ms         

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 1.48 Gbits/sec  | 2.00 Gbits/sec  | 109 ms         
Eranium         | Amsterdam, NL (100G)      | 1.43 Gbits/sec  | 2.12 Gbits/sec  | 114 ms         
Uztelecom       | Tashkent, UZ (10G)        | 699 Mbits/sec   | 904 Mbits/sec   | 206 ms         
Leaseweb        | Singapore, SG (10G)       | 744 Mbits/sec   | 1.09 Gbits/sec  | --             
Clouvider       | Los Angeles, CA, US (10G) | 3.85 Gbits/sec  | 3.64 Gbits/sec  | 31.1 ms        
Leaseweb        | NYC, NY, US (10G)         | 3.91 Gbits/sec  | 3.58 Gbits/sec  | 37.3 ms        
Edgoo           | Sao Paulo, BR (1G)        | busy            | busy            | 142 ms         

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value                         
                |                               
Single Core     | 1642                          
Multi Core      | 4249                          
Full Test       | https://browser.geekbench.com/v6/cpu/19485150

YABS completed in 13 min 43 sec
```

YABS Amsterdam, KVM 7 GB (click to open)

```
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-10-31                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Tue Nov 17 12:59:00 PM UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 0 minutes
Processor  : AMD EPYC 7C13 64-Core Processor
CPU cores  : 3 @ 1999.999 MHz
AES-NI     : ✔️ Enabled
VM-x/AMD-V : ✔️ Enabled
RAM        : 6.8 GiB
Swap       : 0.0 KiB
Disk       : 139.9 GiB
Distro     : AlmaLinux 10.2 (Lavender Lion)
Kernel     : 6.12.0-211.47.1.el10_2.x86_64
VM Type    : KVM
IPv4/IPv6  : ✔️ Online / ✔️ Online

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
Read       | 41.04 MB/s   (10.0k) | 303.42 MB/s   (4.6k)
Write      | 41.14 MB/s   (10.0k) | 305.01 MB/s   (4.6k)
Total      | 82.18 MB/s   (20.0k) | 608.43 MB/s   (9.2k)
           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 297.14 MB/s    (566) | 295.16 MB/s    (281)
Write      | 312.93 MB/s    (596) | 314.82 MB/s    (300)
Total      | 610.08 MB/s   (1.1k) | 609.99 MB/s    (581)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 2.49 Gbits/sec  | 2.33 Gbits/sec  | 6.34 ms        
Eranium         | Amsterdam, NL (100G)      | 2.52 Gbits/sec  | 2.36 Gbits/sec  | 0.321 ms       
Uztelecom       | Tashkent, UZ (10G)        | 1.73 Gbits/sec  | 1.62 Gbits/sec  | 97.0 ms        
Leaseweb        | Singapore, SG (10G)       | 875 Mbits/sec   | 1.36 Gbits/sec  | 175 ms         
Clouvider       | Los Angeles, CA, US (10G) | 1.19 Gbits/sec  | 591 Mbits/sec   | 131 ms         
Leaseweb        | NYC, NY, US (10G)         | 2.01 Gbits/sec  | 1.94 Gbits/sec  | 76.9 ms        
Edgoo           | Sao Paulo, BR (1G)        | busy            | busy            | 196 ms         

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 2.51 Gbits/sec  | 2.30 Gbits/sec  | 7.38 ms        
Eranium         | Amsterdam, NL (100G)      | 2.52 Gbits/sec  | 2.32 Gbits/sec  | 0.773 ms       
Uztelecom       | Tashkent, UZ (10G)        | 1.72 Gbits/sec  | 1.75 Gbits/sec  | 97.1 ms        
Leaseweb        | Singapore, SG (10G)       | 801 Mbits/sec   | 1.21 Gbits/sec  | 190 ms         
Clouvider       | Los Angeles, CA, US (10G) | 1.08 Gbits/sec  | 1.44 Gbits/sec  | 149 ms         
Leaseweb        | NYC, NY, US (10G)         | 2.22 Gbits/sec  | 2.17 Gbits/sec  | 75.4 ms        
Edgoo           | Sao Paulo, BR (1G)        | busy            | busy            | 183 ms         

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value                         
                |                               
Single Core     | 1443                          
Multi Core      | 3679                          
Full Test       | https://browser.geekbench.com/v6/cpu/19485149

YABS completed in 13 min 30 sec
```

See customer feedback from our last LET deal <https://lowendtalk.com/discussion/221558>

Looking glass and test IPs for all three locations <https://www.d4networks.com/looking-glass>  
Questions are welcome here or by ticket.

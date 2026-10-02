---
id: 221687
title: "LayerOne VPS Hosting - Up to 30% off - New NVME Backed Storage + Routed IPv6 Support"
date: "2026-10-02T18:47:36+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/221687/layerone-vps-hosting-up-to-30-off-new-nvme-backed-storage-routed-ipv6-support"
---
# LayerOne VPS Hosting - Up to 30% off - New NVME Backed Storage + Routed IPv6 Support
**Link:** [Original Thread](https://lowendtalk.com/discussion/221687/layerone-vps-hosting-up-to-30-off-new-nvme-backed-storage-routed-ipv6-support)

Hello all!

LayerOne is excited to post our newest offer to LowEndTalk. We now offer **NVMe-backed storage and IPv6 support on all of our plans**.  
(Existing customers can enable IPv6 starting October 31st; new customers get IPv6 on all plans.)

**Exclusive LET pricing: 20% off monthly, 30% off annual**  
Monthly is billed by the hour. Annual is paid upfront as account credit.

All plans include: Enterprise NVMe SSD, 1 dedicated IPv4, IPv6. (Routed /64), DDoS mitigation | Location: Tampa, FL | AS31916

---

### General Compute (2.5 Gbit/s port)

| Plan | vCPU | RAM | NVMe | Monthly | Annual |
| --- | --- | --- | --- | --- | --- |
| gc.nano | 1 | 1 GB | 20 GB | [$2.40/mo](https://layeronecloud.com/client/order/layerone-nano-let-promo-6/?cadence=hourly) | [$20.16/yr](https://layeronecloud.com/client/order/layerone-nano-let-promo-6/?cadence=annual) |
| gc.micro | 1 | 2 GB | 40 GB | [$4.00/mo](https://layeronecloud.com/client/order/layerone-starter-let-promo-6/?cadence=hourly) | [$33.60/yr](https://layeronecloud.com/client/order/layerone-starter-let-promo-6/?cadence=annual) |
| gc.small | 2 | 4 GB | 60 GB | [$6.40/mo](https://layeronecloud.com/client/order/layerone-4g-let-promo-6/?cadence=hourly) | [$53.76/yr](https://layeronecloud.com/client/order/layerone-4g-let-promo-6/?cadence=annual) |

### Network Optimized (10 Gbit/s port)

| Plan | vCPU | RAM | NVMe | Monthly | Annual |
| --- | --- | --- | --- | --- | --- |
| no.appliance | 1 | 512 MB | 20 GB | [$2.40/mo](https://layeronecloud.com/client/order/layerone-no-appliance-let-promo-6/?cadence=hourly) | [$20.16/yr](https://layeronecloud.com/client/order/layerone-no-appliance-let-promo-6/?cadence=annual) |
| no.nano | 1 | 1 GB | 20 GB | [$4.00/mo](https://layeronecloud.com/client/order/layerone-no-nano-let-promo-6/?cadence=hourly) | [$33.60/yr](https://layeronecloud.com/client/order/layerone-no-nano-let-promo-6/?cadence=annual) |
| no.micro | 2 | 2 GB | 40 GB | [$8.00/mo](https://layeronecloud.com/client/order/layerone-no-starter-let-promo-6/?cadence=hourly) | [$67.20/yr](https://layeronecloud.com/client/order/layerone-no-starter-let-promo-6/?cadence=annual) |

All offers: <https://layeronecloud.com/let-promo/>

---

### 🎁 Exclusive LET Bonus

**Comment your VPS ID below and we'll grant you one of the following:**  
- +1 GB additional memory  
- +10 GB additional NVMe storage  
- +1 extra vCPU core

### 🏆 Giveaway

Comment **LAYERONEVPS** along with the VMID of your purchase to be entered to win **6 months of your plan's renewal price as account credit (up to $100)**.

* One winner, applied to one VM
* Drawing takes place **October 31st**

---

**Spoiler: YABS Test (gc.nano, Tampa)**

```
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-09-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Fri Oct  2 16:17:30 UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 27 minutes
Processor  : Intel(R) Xeon(R) Gold 6150 CPU @ 2.70GHz
CPU cores  : 1 @ 2693.670 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 956.3 MiB
Swap       : 0.0 KiB
Disk       : 19.3 GiB
Distro     : Ubuntu 26.04.1 LTS
Kernel     : 7.0.0-31-generic
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        :  LayerOne LLC
ASN        : 31916
Host       : LayerOne LLC
Location   : Tampa, Florida (FL)
Country    : United States

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/sda1):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 239.59 MB/s  (58.4k) | 2.31 GB/s    (35.2k)
Write      | 240.23 MB/s  (58.6k) | 2.32 GB/s    (35.4k)
Total      | 479.83 MB/s (117.1k) | 4.63 GB/s    (70.7k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 4.77 GB/s     (9.1k) | 4.78 GB/s     (4.5k)
Write      | 5.02 GB/s     (9.5k) | 5.10 GB/s     (4.8k)
Total      | 9.80 GB/s    (18.7k) | 9.89 GB/s     (9.4k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 580 Mbits/sec   | 1.84 Gbits/sec  | 117 ms
Eranium         | Amsterdam, NL (100G)      | 665 Mbits/sec   | 2.13 Gbits/sec  | 112 ms
Uztelecom       | Tashkent, UZ (10G)        | 162 Mbits/sec   | 1.28 Gbits/sec  | 209 ms
Leaseweb        | Singapore, SG (10G)       | 479 Mbits/sec   | 1.06 Gbits/sec  | 255 ms
Clouvider       | Los Angeles, CA, US (10G) | 764 Mbits/sec   | 2.15 Gbits/sec  | 72.3 ms
Leaseweb        | NYC, NY, US (10G)         | 504 Mbits/sec   | 2.34 Gbits/sec  | 35.6 ms
Edgoo           | Sao Paulo, BR (1G)        | 102 Mbits/sec   | 1.29 Gbits/sec  | 211 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 729 Mbits/sec   | 102 Mbits/sec   | 118 ms
Eranium         | Amsterdam, NL (100G)      | 312 Mbits/sec   | 1.97 Gbits/sec  | 114 ms
Uztelecom       | Tashkent, UZ (10G)        | 242 Mbits/sec   | 1.16 Gbits/sec  | 209 ms
Leaseweb        | Singapore, SG (10G)       | 431 Mbits/sec   | 964 Mbits/sec   | 267 ms
Clouvider       | Los Angeles, CA, US (10G) | 666 Mbits/sec   | 2.12 Gbits/sec  | 70.5 ms
Leaseweb        | NYC, NY, US (10G)         | 533 Mbits/sec   | 2.26 Gbits/sec  | 34.5 ms
Edgoo           | Sao Paulo, BR (1G)        | busy            | 732 Mbits/sec   | 343 ms
```

---
id: 221054
title: "Caliber Node – Dallas VPS | Xeon Gold | 50Gbps | AS54953 | Limited-Time Bonus"
date: "2026-09-14T18:14:22+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/221054/caliber-node-dallas-vps-xeon-gold-50gbps-as54953-limited-time-bonus"
---
# Caliber Node – Dallas VPS | Xeon Gold | 50Gbps | AS54953 | Limited-Time Bonus
**Link:** [Original Thread](https://lowendtalk.com/discussion/221054/caliber-node-dallas-vps-xeon-gold-50gbps-as54953-limited-time-bonus)

Hi all!

Caliber Node here with a special VPS offer out of **Dallas, Texas**.

Who is Caliber Node?
--------------------

We're a relatively new provider and have been operating for around **2 years**. Our primary focus has been managed application hosting, which has grown considerably for us.

We're now opening up our virtual server offerings because we understand that sometimes you need more than just a managed app — you need the flexibility of a full VPS.

I'm happy to answer any questions as they come up.

Now, let's get to the good stuff!

---

Network & Infrastructure
------------------------

Our Dallas equipment is leased through **MinRTT** and located at **Equinix DA11 in Dallas, Texas**.

We operate our own network under **AS54953**.

Each server has **50Gbps of connectivity**, consisting of **2x 25Gbps links configured in LACP** across dual ToR switches.

Our infrastructure is designed with redundancy throughout:

* Dual ToR switches
* Redundant core switches
* Redundant border routers
* 2x 25Gbps LACP per server
* Redundant NIC connectivity
* Dual A+B power
* Redundant power supplies
* Hot-swap enterprise NVMe drives

---

Network / Test Information
--------------------------

**Location:** Dallas, Texas  
**ASN:** AS54953

**IPv4 Test:** `23.136.172.16`  
**IPv6 Test:** `2604:1c20:806:1::2`

---

Node Specifications
-------------------

| Hardware | Specification |
| --- | --- |
| **CPU** | 2x Intel Xeon Gold 6234 |
| **CPU Resources** | 16 Cores / 32 Threads Total |
| **RAM** | 256GB DDR4 ECC |
| **Storage** | 4x 960GB Enterprise NVMe Gen3 |
| **Network** | 50Gbps – 2x 25Gbps LACP |
| **Switching** | Redundant ToR Switches |
| **Power** | Redundant PSUs / A+B Feeds |

---

Built-In VPS Control Panel
--------------------------

Manage your VPS directly through our custom **Caliber Node control panel**.

Features include:

* **Start, stop, and reboot** your server
* **Browser console** access when SSH or guest networking needs attention
* **OS reinstall** with Ubuntu, Debian, AlmaLinux, or Rocky Linux
* **Root password resets**
* **SSH key management**
* **Firewall management** directly from the panel
* **IPv6 management** with your own `/64` and address generation on supported guests
* **IPv4 reverse DNS / PTR management**
* **Resource usage and monthly transfer monitoring**
* **One manual off-site snapshot slot included per VPS**
* **Additional snapshot slot available as a paid upgrade**
* **Billing, invoices, and support tickets** managed from the same account

These are **self-managed VPSs**. You control the operating system, applications, and software running inside your VPS, while we maintain the underlying hardware, networking, and infrastructure.

---

How to Order
============

Register here to place your VPS order:

**<https://portal.calibernode.com/register>**

**No coupon is needed.**

**Payment Methods:** Credit / Debit Card processed through Stripe.

---

4GB VPS YABS Benchmark
----------------------

**Yet-Another-Bench-Script v2026-07-24**  
<https://github.com/masonr/yet-another-bench-script>

```
Sat Sep 12 15:10:08 UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 0 minutes
Processor  : Intel(R) Xeon(R) Gold 6234 CPU @ 3.30GHz
CPU cores  : 2 @ 3292.234 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 3.8 GiB
Swap       : 0.0 KiB
Disk       : 39.3 GiB
Distro     : Debian GNU/Linux 12 (bookworm)
Kernel     : 6.1.0-52-cloud-amd64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : MinRTT Inc
ASN        : AS401909 MinRTT Inc
Host       : MinRTT Inc
Location   : Austin, Texas (TX)
Country    : United States

fio Disk Speed Tests (Mixed R/W 50/50):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
Read       | 302.40 MB/s  (73.8k) | 2.49 GB/s    (38.0k)
Write      | 303.20 MB/s  (74.0k) | 2.50 GB/s    (38.2k)
Total      | 605.60 MB/s (147.8k) | 4.99 GB/s    (76.2k)

Block Size | 512k          (IOPS) | 1m            (IOPS)
Read       | 4.58 GB/s     (8.7k) | 4.90 GB/s     (4.6k)
Write      | 4.83 GB/s     (9.2k) | 5.22 GB/s     (4.9k)
Total      | 9.41 GB/s    (17.9k) | 10.12 GB/s    (9.6k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider   | Location       | Send           | Receive        | Ping
Clouvider  | London         | 1.58 Gbits/sec | 1.61 Gbits/sec | 110 ms
Eranium    | Amsterdam      | 1.91 Gbits/sec | 1.50 Gbits/sec | 117 ms
Uztelecom  | Tashkent       | 883 Mbits/sec  | 750 Mbits/sec  | 236 ms
Leaseweb   | Singapore      | 8.92 Mbits/sec | 750 Mbits/sec  | 233 ms
Clouvider  | Los Angeles    | 4.65 Gbits/sec | 6.09 Gbits/sec | 30.7 ms
Leaseweb   | New York       | 3.50 Gbits/sec | 4.44 Gbits/sec | 44.0 ms
Edgoo      | Sao Paulo      | 1.50 Gbits/sec | 1.21 Gbits/sec | 137 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider   | Location       | Send           | Receive        | Ping
Clouvider  | London         | 1.56 Gbits/sec | 1.54 Gbits/sec | 112 ms
Eranium    | Amsterdam      | 1.43 Gbits/sec | 1.31 Gbits/sec | 129 ms
Uztelecom  | Tashkent       | busy           | 702 Mbits/sec  | 228 ms
Leaseweb   | Singapore      | 719 Mbits/sec  | 470 Mbits/sec  | 285 ms
Clouvider  | Los Angeles    | 3.84 Gbits/sec | 6.19 Gbits/sec | 31.0 ms
Leaseweb   | New York       | 3.21 Gbits/sec | 4.45 Gbits/sec | 42.7 ms
Edgoo      | Sao Paulo      | busy           | busy           | 256 ms

YABS completed in 9 min 10 sec
```

---

VPS Plans
=========

VPS 1 – $6 / 3 Months
---------------------

**$6.00 every 3 months — $2/month effective**

* **1 Shared vCPU**
* **1GB RAM**
* **10GB NVMe**
* **1TB Monthly Transfer**
* **1 IPv4**
* **/64 IPv6**

---

VPS 2 – $4 / Month
------------------

**$4.00/month**

* **1 Shared vCPU**
* **2GB RAM**
* **20GB NVMe**
* **2TB Monthly Transfer**
* **1 IPv4**
* **/64 IPv6**
* **Monthly Billing**

---

VPS 4 – $6 / Month
------------------

**$6.00/month**

* **2 Shared vCPU**
* **4GB RAM**
* **40GB NVMe**
* **3TB Monthly Transfer**
* **1 IPv4**
* **/64 IPv6**
* **Monthly Billing**

---

Limited-Time Bonus – Free Micro Apps Plan
=========================================

For a limited time, VPS customers can also receive one of our **Micro Apps plans completely FREE**.

After ordering, simply **comment your invoice number in this thread** and we'll add the Micro Apps plan to your account.

Your free Micro Apps plan includes:

* **1 vCPU**
* **1GB RAM**
* **15GB Storage**
* Access to **200+ one-click applications**

This is completely separate from your VPS and gives you access to our managed application platform at **no additional cost**.

Deploy apps without having to manage the underlying server, Docker configuration, SSL, or other infrastructure yourself.

---

Company Information
-------------------

**Caliber Node, LLC**  
North Carolina SOSID: **3011683**

PMB 415  
1236 NC Highway 210  
Sneads Ferry, NC 28460  
United States

---

Questions about the network, hardware, VPSs, benchmarks, or our app platform? Feel free to ask.

Thanks for checking us out!

**Caliber Node, LLC**  
**AS54953**

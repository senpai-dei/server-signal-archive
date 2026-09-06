---
id: 220847
title: "Blackbox : 2 vCPU / 4 GB / 50 GB NVMe, Encrypted RAM & Disk, 100% Anonymous - $9.99/mo"
date: "2026-09-06T08:33:47+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/220847/blackbox-2-vcpu-4-gb-50-gb-nvme-encrypted-ram-disk-100-anonymous-9-99-mo"
---
# Blackbox : 2 vCPU / 4 GB / 50 GB NVMe, Encrypted RAM & Disk, 100% Anonymous - $9.99/mo
**Link:** [Original Thread](https://lowendtalk.com/discussion/220847/blackbox-2-vcpu-4-gb-50-gb-nvme-encrypted-ram-disk-100-anonymous-9-99-mo)

Matteo again, from Servury. Two weeks ago I posted Blackbox, the VPS whose operator cannot read its memory, cannot read its disk, and cannot run commands inside it. Thread [here](https://lowendtalk.com/discussion/220383/servury-blackbox-zero-knowledge-vps-encrypted-ram-encrypted-disk-and-no-guest-agent-from-9-99/p1 "here"). Since then we shipped the things people in that thread asked about, and re-specced the entry plan.

What changed since the last thread

1. Core is now 2 vCPU / 4 GB / 50 GB NVMe, same $9.99. The 1 vCPU / 512 MB Core is gone. If you bought one, your VM already has 4 GB queued: all you have to do is ask us via support to bump your specs up.
2. Measured boot. In the last thread the honest limit was "you're still trusting our boot image." Not any more. The firmware, kernel and initramfs are built reproducibly from public source, the expected launch measurement is published for every release, and an open verifier recomputes it and checks it against the CPU-signed attestation report your own machine hands you over SSH, before you type a LUKS passphrase. The guide, the source tarball and the verifier: <https://servury.com/docs/guides/measured-boot/>
3. Our own control plane. New Blackbox machines run on QEMU/KVM under a wrapper we wrote (Rust, one systemd unit per guest). No Proxmox, Virtualizor or VirtFusion in the path. Every guest is an unprivileged process with an empty capability set, seccomp, a private mount namespace where it cannot see another guest's sockets or disks, a device allowlist, private PIDs, and no ability to open a network socket of its own. SEV-SNP protects you from the host; this is what protects you from a neighbour who escapes QEMU.
4. Custom ISO from any URL, attached as a CD, boots first when you say so.
5. Console logging is off by default, and it's a per-VM switch on the Console tab. Nothing your kernel prints to the serial port is written on the host unless you turn it on.
6. Abuse reports are read by a person before anything happens, on every plan, not just the top one.

Everything from the first thread still holds: no guest agent and no port for one, LUKS you unlock yourself over dropbear, /dev/sev-guest exposed so you pull the attestation report from the silicon, no email, no phone, no KYC, 11 cryptocurrencies through our own processor or Stripe or cash by mail, zero access logs anywhere including the looking glass, and the site works with JavaScript off. BYOIP, self-managed rDNS - I could go on.

Plan

Blackbox Core - $9.99/month, $29.97/quarter (USD). Any term from 7 to 365 days, prorated.  
2 vCPU, AMD EPYC 7543 | 4 GB RAM, SEV-SNP encrypted | 50 GB NVMe on a ZFS mirror  
1 dedicated IPv4 + routed /64 | 10 Gbps unmetered | KVM, full root, UEFI  
Montreal, Cologix MTL2, our hardware, AS395904, 23.155.44.0/24, 2602:f41c::/36  
Templates: Debian 12/13, Ubuntu 24.04/26.04, Rocky 9, AlmaLinux 9/10, FreeBSD 14/15, OpenBSD 7.8/7.9  
Order: <https://servury.com/>

Bigger tiers exist on the site (up to 8 vCPU / 32 GB / 400 GB). Stock note, since I'd rather say it here than have you find out at checkout: the node is nearly full, Core and the next tier up are available now, the two larger ones return after the RAM upgrade landing next week, and lots more stock when we'll rack the second node at the end of the month.

Looking glass, test IPs, test files

<https://mtl-lg.servury.com>  
IPv4: 23.155.44.21 | IPv6: 2602:f41c:0:a::1  
Test files: 100 MB / 1 GB / 10 GB  
iperf3 -c mtl-lg.servury.com -p 5201 -P 4 (add -R for the other direction)  
No access log, no visitor IPs recorded, Bootstrap served from our own host.

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

Network summary from that run:  
NYC 9.34 / 9.35 Gbit/s, 9.8 ms | Los Angeles 3.33 / 4.15, 57 ms | London 2.19 / 3.00, 71 ms | Amsterdam 2.66 / 3.10, 80 ms | Sao Paulo 1.57 / 2.01, 117 ms

Terms: <https://servury.com/terms/> (illegal content, CSAM, fraud, attacks, spam, mining and IP infringement get you suspended without refund; abuse reports from law enforcement with valid process, NCMEC, transit and valid DMCA are handled by a human).

Contact: <https://servury.com> | [[email protected]](/cdn-cgi/l/email-protection) | here

Feedback is heavily appreciated, chances are - if you have a good idea, we'll make it a thing ![:)](https://lowendtalk.com/resources/emoji/smile.png ":)")

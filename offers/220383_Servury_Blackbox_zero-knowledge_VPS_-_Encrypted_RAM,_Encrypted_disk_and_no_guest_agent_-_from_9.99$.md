---
id: 220383
title: "Servury Blackbox zero-knowledge VPS - Encrypted RAM, Encrypted disk and no guest agent - from 9.99$"
date: "2026-08-22T23:06:15+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/220383/servury-blackbox-zero-knowledge-vps-encrypted-ram-encrypted-disk-and-no-guest-agent-from-9-99"
---
# Servury Blackbox zero-knowledge VPS - Encrypted RAM, Encrypted disk and no guest agent - from 9.99$
**Link:** [Original Thread](https://lowendtalk.com/discussion/220383/servury-blackbox-zero-knowledge-vps-encrypted-ram-encrypted-disk-and-no-guest-agent-from-9-99)

I'm Matteo, I run Servury, a 100% anonymous VPS/VDS provider platform. Today, I'm thrilled to present to you our new product - Blackbox, which I believe is the first of it's kind. It's a zero knowledge VPS, where even we (the hypervisor) can't read your VM's memory, disk, or run arbitrary commands inside of it.

**Every hosting provider on this forum can do three things to your VPS.** They can dump your RAM from the hypervisor. They can execute commands inside your guest without your SSH key. And they can read your disk by mounting it from the host. That is not a knock on anyone - it is simply how virtualisation works, and every provider here, including the big ones, sits in that position whether they want to or not.

**This is a box where we can't do any of the three.** Not "we promise not to" or "we have a policy". The capability is removed, and you can verify all of it from inside your own VM.

**We are not the cheapest box on this forum and we're not trying to be.** If you want 4 GB for $20/year, that offer exists and it isn't this one. What you're paying for is a machine its operator cannot look inside.

---

The three things, and how you check them yourself
-------------------------------------------------

### 1. We can't read your memory

AMD SEV-SNP. Your guest's RAM is encrypted with a key that lives in the CPU's security processor.

```
$ dmesg | grep -i "Memory Encryption"
Memory Encryption Features active: AMD SEV SEV-ES SEV-SNP

$ dmesg | grep VMPL
SEV: SNP running at VMPL0.
```

And you don't have to take that output on faith either, because the attestation device is exposed to you:

```
$ ls -l /dev/sev-guest
crw------- 1 root root 10, 262 /dev/sev-guest
```

That is the interface to the AMD PSP. You can pull a **signed attestation report** from the silicon and check it against AMD's root of trust yourself. We cannot forge it and we cannot intercept it.

### 2. We can't reach into your guest

Nearly every VPS you have ever rented runs a **guest agent** - a daemon inside your VM listening on a virtio serial port, which lets the host run commands as root inside your guest, read arbitrary files, and reset your password. It is how "reset root password" works in a control panel. It is enabled by default in Proxmox, and both Azure and GCP keep their agents running inside confidential VMs too.

**On a Servury Blackbox there is no agent, and no port for one.** It isn't disabled in software where it could be switched back on - the virtio-serial device is absent from the QEMU command line entirely. From inside your VM:

```
$ ls /dev/virtio-ports/ 2>/dev/null
(nothing - there is no org.qemu.guest_agent.0)
```

Because the channel does not exist, "reset my root password from the panel" is a feature we genuinely cannot offer you on a Blackbox VM. If we have the ability to reset your root password, you're forced to trust we won't tamper with your VM at any given time, which is utter garbage in our opinion. Don't trust, verify.

### 3. We can't read your disk

Optional LUKS full-disk encryption, unlocked over SSH by dropbear in the initramfs. You set the passphrase yourself on first boot and it never touches our systems. Combined with the above: your disk is ciphertext at rest, your RAM is ciphertext in use, and the key exists only in encrypted memory we can't read.

### And we don't know who you are

No email, no phone, no KYC. Signup hands you a credential and that is the whole account. Payment is 11 coins through **our own** processor - our node, our watcher, no third party in the middle collecting your addresses and your IP - or Stripe, or cash by mail.

**Zero logs.** No access logs anywhere on the platform, including the looking glass below. This is the only thing you can't really verify. See Trusting Trust (Ken Thompson, 1984). We'll be looking into getting an audit done in the future.

**No-JS Compatible.** Servury is designed to work with JS disabled. For people who pay with credit cards, we only load the Stripe assets when credit card is explicitely selected as a payment method.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Kickass features
----------------

**We own the whole stack.** AS395904, `23.155.44.0/24`, `2602:f41c::/36`, our own switch, our  
own hardware at Cologix MTL2. If you traceroute the looking glass you are looking at the same path your VM sits behind, because it is literally an address out of the same /24 your VM gets assigned from.

**BYOIP** Bring your own prefix and we announce it from AS395904, v4 and v6, as buttons in the panel rather than a ticket. RPKI verification is automated.

**rDNS** you set yourself, in the panel, not by ticket.

**12 OS templates**, all UEFI, all built by hand: Debian 12/13, Ubuntu 24.04/26.04, Rocky 9, AlmaLinux 9/10, FreeBSD 14/15, OpenBSD 7.8/7.9, Windows Server 2025.

**Manual abuse report handling**, on the Pro tier.

**Priority human support**, from me, the founder. On the pro tier you get my cellphone number.

---

Plans
-----

Both plans are on the Montreal node (Cologix MTL2). Every plan: **1 dedicated IPv4 + a routed /64 IPv6**, 10 Gbps unmetered, NVMe on a ZFS mirror, full root, KVM.

| Plan | vCPU | RAM | Disk | Price |
| --- | --- | --- | --- | --- |
| **Blackbox Core** | 1 | 512 MB | 50 GB NVMe | **$9.99/mo** |

Order: <https://servury.com>

**Need something bigger?** The nodes are 32c/64t EPYC with 250 GB of RAM and 7 TB of NVMe, so there is a lot of room above the Pro plan. I'll build a custom spec - more cores, more RAM, a big volume, whatever you actually need - **on 6 months prepaid**. Tell me the spec and I'll quote it in the thread so everyone can see the number.

---

Looking glass, test IPs, test files
-----------------------------------

**<https://mtl-lg.servury.com>**

* Looking glass IPv4: `23.155.44.21`
* Looking glass IPv6: `2602:f41c:0:a::1`
* Test files: [100 MB](https://mtl-lg.servury.com/100MB.bin) / [1 GB](https://mtl-lg.servury.com/1GB.bin) / [10 GB](https://mtl-lg.servury.com/10GB.bin)
* iperf3: `iperf3 -c mtl-lg.servury.com -p 5201 -P 4` (add `-R` for the other direction)

The looking glass keeps **no access log** and records no visitor IP addresses - same as the rest of the platform. It also serves Bootstrap from our own host rather than a CDN, so opening it doesn't hand your address to a third party either.

---

YABS
----

### Blackbox Pro - 2 vCPU / 4 GB / 50 GB

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

### Blackbox Core - 1 vCPU / 512 MB / 50 GB

Geekbench : **GB6 does not fit in 512 MB**.

```
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-07-24                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Fri Aug 21 01:19:20 AM UTC 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 1 minutes
Processor  : AMD EPYC-v4 Processor
CPU cores  : 1 @ 2794.748 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ❌ Disabled
RAM        : 396.8 MiB
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
Read       | 156.08 MB/s  (38.1k) | 1.77 GB/s    (27.0k)
Write      | 156.50 MB/s  (38.2k) | 1.77 GB/s    (27.1k)
Total      | 312.58 MB/s  (76.3k) | 3.54 GB/s    (54.1k)
           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 6.43 GB/s    (12.2k) | 7.66 GB/s     (7.3k)
Write      | 6.77 GB/s    (12.9k) | 8.17 GB/s     (7.8k)
Total      | 13.21 GB/s   (25.2k) | 15.84 GB/s   (15.1k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           

Clouvider       | London, UK (10G)          | 2.00 Gbits/sec  | 1.62 Gbits/sec  | 71.2 ms        

Eranium         | Amsterdam, NL (100G)      | 1.44 Gbits/sec  | 1.42 Gbits/sec  | 80.2 ms        

Uztelecom       | Tashkent, UZ (10G)        | 805 Mbits/sec   | 633 Mbits/sec   | 169 ms         

Leaseweb        | Singapore, SG (10G)       | 504 Mbits/sec   | 428 Mbits/sec   | 241 ms         

Clouvider       | Los Angeles, CA, US (10G) | 2.48 Gbits/sec  | 2.03 Gbits/sec  | 57.0 ms        

Leaseweb        | NYC, NY, US (10G)         | 9.28 Gbits/sec  | 9.14 Gbits/sec  | 9.61 ms        

Edgoo           | Sao Paulo, BR (1G)        | 1.11 Gbits/sec  | 976 Mbits/sec   | 117 ms         

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           

Clouvider       | London, UK (10G)          | 2.02 Gbits/sec  | 1.58 Gbits/sec  | 70.7 ms        

Eranium         | Amsterdam, NL (100G)      | 1.85 Gbits/sec  | 1.38 Gbits/sec  | 80.2 ms        

Uztelecom       | Tashkent, UZ (10G)        | 863 Mbits/sec   | 577 Mbits/sec   | 169 ms         

Leaseweb        | Singapore, SG (10G)       | 500 Mbits/sec   | 407 Mbits/sec   | 249 ms         

Clouvider       | Los Angeles, CA, US (10G) | 2.39 Gbits/sec  | 1.92 Gbits/sec  | 57.8 ms        

Leaseweb        | NYC, NY, US (10G)         | 8.98 Gbits/sec  | 9.21 Gbits/sec  | 10.1 ms        

Edgoo           | Sao Paulo, BR (1G)        | 1.15 Gbits/sec  | busy            | 118 ms         

YABS completed in 7 min 5 sec
```

Network summary, from the Pro run - Montreal is a good place to sit if you care about the US  
northeast:

| Destination | Send | Recv | Ping |
| --- | --- | --- | --- |
| NYC | 9.34 Gbit/s | 9.35 Gbit/s | 9.8 ms |
| Los Angeles | 3.33 Gbit/s | 4.15 Gbit/s | 57 ms |
| London | 2.19 Gbit/s | 3.00 Gbit/s | 71 ms |
| Amsterdam | 2.66 Gbit/s | 3.10 Gbit/s | 80 ms |
| Sao Paulo | 1.57 Gbit/s | 2.01 Gbit/s | 117 ms |

---

Terms
-----

Prohibited: anything illegal, CSAM, fraud/phishing, unauthorised attacks on other systems,  
spam, **cryptocurrency mining**, and IP infringement. Violations mean suspension without refund.

We process abuse reports from law enforcement with valid legal process, NCMEC, our network  
transit, and valid DMCA notices.

Full terms: <https://servury.com/terms/>

---

Contact
-------

* Web: <https://servury.com>
* Email: [[email protected]](/cdn-cgi/l/email-protection)
* Here

Happy to run any test you want on the looking glass, and if there's a specific YABS variant or a benchmark you'd like to see on one of these plans, ask and I'll post it.

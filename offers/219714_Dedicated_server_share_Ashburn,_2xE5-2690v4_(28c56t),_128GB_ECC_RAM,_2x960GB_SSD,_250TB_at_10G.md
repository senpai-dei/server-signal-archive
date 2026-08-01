---
id: 219714
title: "Dedicated server share: Ashburn, 2xE5-2690v4 (28c/56t), 128GB ECC RAM, 2x960GB SSD, 250TB at 10G"
date: "2026-08-01T22:22:03+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/219714/dedicated-server-share-ashburn-2xe5-2690v4-28c-56t-128gb-ecc-ram-2x960gb-ssd-250tb-at-10g"
---
# Dedicated server share: Ashburn, 2xE5-2690v4 (28c/56t), 128GB ECC RAM, 2x960GB SSD, 250TB at 10G
**Link:** [Original Thread](https://lowendtalk.com/discussion/219714/dedicated-server-share-ashburn-2xe5-2690v4-28c-56t-128gb-ecc-ram-2x960gb-ssd-250tb-at-10g)

Hello!

From the old days, even long before [MetalVPS.com](https://metalvpscom) started in 2020, I have shared shell accounts on my servers. I've had tons of fun learning a little from the guys with whom I have shared!

Shell accounts on a new-to-me, rented from [Quickpacket](https://quickpacket.com), dual E5 Ashburn server presently might be available if anyone here wants both to share the server with me and to help fund it.

**Specifications**

* 2 x E5-2690v4 (28c/56t),
* 128 GB DDR4 ECC RAM,
* 2 x 960 GB SSD,
* 1 x IPv4, more available,
* 1 x IPv6/64 and 1 x IPv6/48 HE Tunnelbroker.net,
* 250TB at 10G,
* FreeBSD-16.0-CURRENT,
* ZRAID 1,
* Ashburn, VA USA, and
* $85/month.

What I recently have been doing on the server is following and, once or twice a week, self-bulding FreeBSD-16.0-CURRENT. Here is example compile output:

```
root@qp:/usr/src # grep '>>>' nohup.out | grep -v gtest | grep -v gmock
>>> World build started on Sat Aug  1 04:13:49 UTC 2026
>>> Rebuilding the temporary build tree
>>> stage 1.1: legacy release compatibility shims
>>> stage 1.2: bootstrap tools
>>> Deleting stale dependencies...
>>> Deleting stale dependencies...
>>> stage 2.3: build tools
>>> stage 3: cross tools
>>> stage 3.1: recording build metadata
>>> stage 4.1: building includes
>>> stage 4.2: building libraries
>>> stage 4.3.1: building lib32 shim libraries
>>> stage 4.4: building everything
>>> World build completed on Sat Aug  1 04:59:12 UTC 2026
>>> World built in 2723 seconds, ncpu: 56, make -j56
>>> Kernel build for GENERIC started on Sat Aug  1 04:59:12 UTC 2026
>>> stage 1: configuring the kernel
>>> stage 2.3: build tools
>>> stage 3.1: building everything
>>> Kernel build for GENERIC completed on Sat Aug  1 05:01:58 UTC 2026
>>> Kernel(s)  GENERIC built in 166 seconds, ncpu: 56, make -j56
root@qp:/usr/src #
```

Besides following FreeBSD-CURRENT, I have been learning a little about testing network performance with iperf3 and optimizing via sysctl.

I might add a web server. Maybe an SMTP server too. Maybe VPS hosting capabilities.

A long term goal continues: learn a little about C, assembly, and sh.

Thanks everyone! ![<3](https://lowendtalk.com/resources/emoji/heart.png "<3") Best wishes! ![<3](https://lowendtalk.com/resources/emoji/heart.png "<3")

**How to Get Shell Access**

Please post in this thread:

What are you working on?  
Do you have a website?   
Do you have a source code repository?   
What do you want to run on our server?  
How much server resources will you use?  
How extensively do you want to fund our server's $85/month cost?  
Do Paypal and Zelle work for you?

**Terms of Service**

Free and open source software only.  
White hat only.  
For computer education and fun!  
Not for commercial use.  
No service level agreement.

**Warnings!**

Ephemeral. Could disappear at any moment!  
*Clueless™* Administrator - ZFS and FreeBSD noob!

---
id: 223203
title: "Low End Dedicated Server Share, Vint Hill, Virginia, USA"
date: "2026-11-13T20:55:29+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/223203/low-end-dedicated-server-share-vint-hill-virginia-usa"
---
# Low End Dedicated Server Share, Vint Hill, Virginia, USA
**Link:** [Original Thread](https://lowendtalk.com/discussion/223203/low-end-dedicated-server-share-vint-hill-virginia-usa)

Friendly greetings!

[MetalVPS](https://metalvps.com) now has a new Low End dedicated server, an [OVH SYS-LE-1.](https://eco.us.ovhcloud.com/soyoustart/sys-le-1/)

From shell accounts on this server, we can work directly on the bare metal. Of course, we also can see how well the server node is performing.

[Incus](https://linuxcontainers.org/incus/) has been installed. From shell accounts, with Incus, we easily can launch Linux containers and/or our own KVM VPSes with many Linux distributions and almost any BSD or other custom operating systems. Both the container and KVM launch processes are simple:

```
# Debian Linux Container
debian@vh:~$ incus launch images:debian/13 test-container
# Debian KVM Virtual Machine
debian@vh:~$ incus launch images:debian/13 test-vm --vm
# NetBSD 11.0 Virtual Machine
debian@vh:~$ incus launch images:netbsd/11.0 my-netbsd11 --vm
```

**Sudo**

Sudo is not necessary to make VPSes and containers. Nevertheless, presently, there are two neighbors, myself ( Tom, [@Not\_Oles](https://lowendtalk.com/profile/Not_Oles) ), and another forum member. We both have sudo. However, the other forum member has kindly offered to give up sudo if someone comes aboard who objects to anyone besides me having sudo. Alternatively, if someone else comes aboard who wants sudo, we can consider adding our new neighbor to the sudo group.

**Limits**

There are no limits on number of containers and KVM VPSes per account. There are no per account limits on processor cores, RAM, disk, or bandwidth.

**Current Usage**

```
Not_Oles@vh:~$ date
Thu Nov 12 01:59:30 UTC 2026
Not_Oles@vh:~$ uptime
 01:59:33 up 6 days, 23:58,  1 user,  load average: 0.00, 0.00, 0.00
Not_Oles@vh:~$
```

**Supporting LET**

Hopefully this thread could support LET with positive and helpful conversations! Let's try!

**Specifications**

Intel Xeon D-2123iT  
4 cores; 8 threads  
32 GB DDR4 ECC RAM  
2 x 4 TB SATA HDD  
Debian 13.7  
ZFS RAID 1  
1 x IPv4/32 (More available); IPv6/64  
500 Mbits/sec unmetered  
Vint Hill, Virginia USA  
Cost paid by [@Not\_Oles](https://lowendtalk.com/profile/Not_Oles) to OVH $25/month with a $25 setup fee

**Shell Account Pricing**

$15.00/month

**PayPal Payment Link**

Paypal payment link ($15.00):

<https://www.paypal.com/ncp/payment/C9FSY6ZWXRY42>

**How to Get Access**

Please post in this thread.   
Please remember to post or send your ssh public key.

**Terms of Service**

Free and open source software only.  
White hat only.  
For computer education and fun!  
Not for commercial use.  
No service level agreement.  
No control panel.

**Warnings!**

Ephemeral. Could disappear at any moment!  
*Clueless™* Administrator!

**[**Hetrix Tools**](https://hetrixtools.com) Uptime Ping Monitors**

* [IPv6](https://hetrixtools.com/report/uptime/0feef8f3cb649b73bc9e3dd647ead2fe/)
* [IPv4](https://hetrixtools.com/report/uptime/d8704fa8b5048a43972324994ad746bc/)

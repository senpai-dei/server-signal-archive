---
id: 220489
title: "[Hostodo] Resource Pools are live — split one VPS budget into multiple KVM servers"
date: "2026-08-26T05:19:07+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/220489/hostodo-resource-pools-are-live-split-one-vps-budget-into-multiple-kvm-servers"
---
# [Hostodo] Resource Pools are live — split one VPS budget into multiple KVM servers
**Link:** [Original Thread](https://lowendtalk.com/discussion/220489/hostodo-resource-pools-are-live-split-one-vps-budget-into-multiple-kvm-servers)

Hi LET. We built Resource Pools.

Buy one Hostodo capacity subscription, then create multiple KVM VPSes from the same RAM / disk / IPv4 pool.

No promo code needed for these two launch pools.

Order / manage pools:  
<https://console.hostodo.com/instances?utm_source=lowendtalk&utm_medium=forum&utm_campaign=resource_pools_launch&utm_content=thread>

### What this is

Instead of buying one fixed VPS at a time, you buy account capacity:

* pooled RAM
* pooled NVMe disk
* VM slots
* included public IPv4s
* create / delete pool VMs for $0 while inside quota

Good for labs, dev boxes, monitoring nodes, small customer environments, or anyone who wants multiple real public servers without managing separate subscriptions for every tiny VM.

### Launch pools

AMD EPYC · KVM · NVMe · 1Gbps · public IPv4 per VM

| Pool | RAM pool | NVMe pool | Max vCPU / VM | VM slots | IPv4s | Price |
| --- | --- | --- | --- | --- | --- | --- |
| Nano | 4GB | 80GB | 2 | 2 | 2 | $5/mo |
| Starter | 8GB | 160GB | 2 | 4 | 4 | $10/mo |

### Examples

Nano gives you 4GB RAM / 80GB NVMe / 2 IPv4s.

You could run:

* 2 × 2GB VMs
* 1 × 4GB VM
* smaller mixed shapes as long as you stay inside pool quota

Starter gives you 8GB RAM / 160GB NVMe / 4 IPv4s.

You could run:

* 4 × 2GB VMs
* 2 × 4GB VMs
* 1 × 8GB VM
* smaller mixed shapes as long as you stay inside pool quota

Create and destroy VMs inside the pool without opening a new invoice every time.

### Locations

Las Vegas, NV  
Detroit, MI  
Tampa, FL

Subject to live regional capacity / IPv4 availability.

Network tests:

Detroit: <https://det01.hostodo.com>  
Las Vegas: <https://lv.hostodo.com>  
Tampa: <https://tpa.hostodo.com>

### CLI + MCP

Resource Pools work in the console.

MCP support is live, so AI agents can list pool options, inspect usage, and create VMs inside a pool.

odo CLI support is released in v2.2.1:

```
brew install hostodo/tap/odo
odo login
odo pools list
odo pools show <pool_id>
```

Create a VM inside a pool:

```
odo instances deploy \
  --pool pool::yourpoolid \
  --os "Ubuntu 24.04" \
  --region DET01 \
  --plan EPYC-2G1C32GN \
  --hostname web-1 \
  --yes
```

### OS options

Ubuntu 25.04 / 24.04 / 22.04  
Debian 13 / 12 / 11  
AlmaLinux 9 / 8  
Rocky Linux 9 / 8  
CentOS Stream 9  
Fedora 43 / 41  
Arch Linux  
OpenSUSE Leap 15.5  
And more.

Unmanaged. Instant provisioning. Stripe, PayPal, Crypto, and Alipay.

Questions here or [[email protected]](/cdn-cgi/l/email-protection)

* Hassan

---
id: 221448
title: "Hostodo Resource Pools - 3 Locations,  many NVMe KVM VPS from one plan - 8G 160G"
date: "2026-09-25T06:56:20+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/221448/hostodo-resource-pools-3-locations-many-nvme-kvm-vps-from-one-plan-8g-160g"
---
# Hostodo Resource Pools - 3 Locations,  many NVMe KVM VPS from one plan - 8G 160G
**Link:** [Original Thread](https://lowendtalk.com/discussion/221448/hostodo-resource-pools-3-locations-many-nvme-kvm-vps-from-one-plan-8g-160g)

Hi LET!

Hassan here from Hostodo.

We built **Resource Pools**, and they’re live.

One capacity plan. Multiple real KVM VPSes. Create them, wipe them, reshape them. No new invoice every time you need another box.

If you want labs, staging, monitoring nodes, client sandboxes, or a bunch of small public servers without stacking separate VPS bills, this is for you.

Order here:  
<https://console.hostodo.com/pools/checkout?utm_source=lowendtalk&utm_medium=forum&utm_campaign=resource_pools_offer&utm_content=thread>

### The offer

AMD EPYC · KVM · Pure NVMe · 1Gbps · dedicated public IPv4 per VM

| Pool | RAM pool | NVMe pool | Max vCPU / VM | VM slots | IPv4s | Price |
| --- | --- | --- | --- | --- | --- | --- |
| **Nano** | 4GB | 80GB | 2 | 2 | 2 | **$5/mo** |
| **Starter** | 8GB | 160GB | 2 | 4 | 4 | **$10/mo** |

No promo code. Recurring as listed.

### What you can actually run

**Nano ($5/mo)** — 4GB RAM / 80GB NVMe / 2 IPv4s

* 2 × 2GB VMs
* 1 × 4GB VM
* or mix smaller shapes inside the pool

**Starter ($10/mo)** — 8GB RAM / 160GB NVMe / 4 IPv4s

* 4 × 2GB VMs
* 2 × 4GB VMs
* 1 × 8GB VM
* or mix smaller shapes inside the pool

Spin VMs up and down inside the pool whenever you want. Stay under quota and it stays on that one subscription.

### Locations

* Las Vegas, NV
* Detroit, MI
* Tampa, FL

Subject to live regional capacity / IPv4 availability.

Network tests:

* Detroit: <https://det01.hostodo.com>
* Las Vegas: <https://lv.hostodo.com>
* Tampa: <https://tpa.hostodo.com>

### Why it’s fun

* One bill, many public KVM servers
* Full root on every VM
* Pure NVMe on AMD EPYC 7742
* Instant provisioning
* Works in console, CLI, and MCP
* AI agents can deploy into your pool too

### CLI + MCP

```
https://api.hostodo.com/mcp
```

```
claude mcp add --transport http --scope user hostodo https://api.hostodo.com/mcp
```

```
hermes mcp add hostodo --url https://api.hostodo.com/mcp
```

```
codex mcp add hostodo --url https://api.hostodo.com/mcp
```

```
brew install hostodo/tap/odo
odo login
odo pools list
odo pools show <pool_id>
```

Deploy into a pool:

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

Unmanaged. Instant. Stripe, PayPal, Crypto, Alipay.

Own network: AS399804. Hosting since late 2014.

Questions here or open a ticket in the console!

* Hassan

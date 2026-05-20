---
id: 217440
title: "[Hostodo] odo CLI public beta - deploy NVMe KVM VPS from your terminal 2G2C 32GB NVMe $29.75/yr"
date: "2026-05-20T07:28:32+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/217440/hostodo-odo-cli-public-beta-deploy-nvme-kvm-vps-from-your-terminal-2g2c-32gb-nvme-29-75-yr"
---
# [Hostodo] odo CLI public beta - deploy NVMe KVM VPS from your terminal 2G2C 32GB NVMe $29.75/yr
**Link:** [Original Thread](https://lowendtalk.com/discussion/217440/hostodo-odo-cli-public-beta-deploy-nvme-kvm-vps-from-your-terminal-2g2c-32gb-nvme-29-75-yr)

Hi LET. We built a CLI. Come check it out!

![](https://media.hostodo.com/promotional/odo-cli-launch-screenshot.png)

```
brew install hostodo/tap/odo
odo login
odo deploy --promo LETCLI
odo ssh my-server
```

Or fully scriptable:

```
odo deploy \
  --os "Ubuntu 24.04" \
  --region DET01 \
  --plan EPYC-8G3C128GN \
  --billing-cycle monthly \
  --promo LETCLI \
  --yes
```

---

### odo CLI

odo is the official Hostodo CLI.

Deploy VPSes, SSH by hostname, manage invoices, add SSH keys, and script provisioning without opening the browser.

Open source:  
<https://github.com/hostodo/odo-cli>

Feedback welcome here or as a GitHub issue.

---

### LETCLI

`LETCLI` = 15% off recurring

Works at checkout or directly in the CLI:

```
odo deploy --promo LETCLI
```

---

### Plans with LETCLI

AMD EPYC 7742 · Pure NVMe · 1Gbps · KVM

| Plan | vCPU | RAM | NVMe | Monthly with LETCLI | Annual with LETCLI |
| --- | --- | --- | --- | --- | --- |
| EPYC-1G1C16GN | 1 | 1GB | 20GB | — | [$17/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-1G1C16GN?promocode=LETCLI) |
| EPYC-2G1C32GN | 2 | 2GB | 32GB | [$2.98/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-2G1C32GN?promocode=LETCLI) | [$29.75/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-2G1C32GN?promocode=LETCLI) |
| EPYC-4G2C64GN | 2 | 4GB | 64GB | [$5.95/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-4G2C64GN?promocode=LETCLI) | [$59.50/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-4G2C64GN?promocode=LETCLI) |
| EPYC-8G3C128GN | 3 | 8GB | 128GB | [$7.65/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-8G3C128GN?promocode=LETCLI) | [$76.50/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-8G3C128GN?promocode=LETCLI) |

---

### Locations

| Location | Test |
| --- | --- |
| Detroit, MI | <https://det01.hostodo.com> |
| Las Vegas, NV | <https://lv.hostodo.com> |
| Tampa, FL | <https://tpa.hostodo.com> |

---

### OS options

Ubuntu 25.04 / 24.04 / 22.04  
Debian 13 / 12 / 11  
AlmaLinux 9 / 8  
Rocky Linux 9 / 8  
CentOS Stream 9  
Fedora 43   
Arch Linux  
OpenSUSE Leap 15.5  
And more

---

Unmanaged. Instant provisioning. Stripe, PayPal, Crypto, and Alipay.

Around since 2014.

Questions here or via helpdesk in the console.

Hassan

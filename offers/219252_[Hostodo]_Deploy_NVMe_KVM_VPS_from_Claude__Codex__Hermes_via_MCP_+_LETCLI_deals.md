---
id: 219252
title: "[Hostodo] Deploy NVMe KVM VPS from Claude / Codex / Hermes via MCP + LETCLI deals"
date: "2026-07-18T12:57:39+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/219252/hostodo-deploy-nvme-kvm-vps-from-claude-codex-hermes-via-mcp-letcli-deals"
---
# [Hostodo] Deploy NVMe KVM VPS from Claude / Codex / Hermes via MCP + LETCLI deals
**Link:** [Original Thread](https://lowendtalk.com/discussion/219252/hostodo-deploy-nvme-kvm-vps-from-claude-codex-hermes-via-mcp-letcli-deals)

![Claude deploying a Hostodo VPS over MCP](https://media.hostodo.com/mcp-deploy-claude-demo.png)

Hi LET. We added MCP support for Hostodo. Since last time, we've simplified the auth flow. Now supporting instance deployment through the MCP.

You can now connect Claude Code, Hermes, Codex, Cursor, OpenCode, or any MCP HTTP client to Hostodo and have your AI agent deploy and manage your instances directly.

---

How to use:
-----------

First, sign up at <https://console.hostodo.com/signup>

**MCP endpoint:**

```
https://api.hostodo.com/mcp
```

**Connect Claude Code**

```
claude mcp add --transport http --scope user hostodo https://api.hostodo.com/mcp
```

Then run `/mcp` inside Claude Code, select `hostodo`, authenticate in your browser, and approve the scopes you want.

**Connect Hermes**

```
hermes mcp add hostodo --url https://api.hostodo.com/mcp
```

**Connect Codex**

```
codex mcp add hostodo --url https://api.hostodo.com/mcp
```

**What Hostodo MCP can do today**

Current production MCP tools include:

* List available regions, plans, OS templates, SSH keys, and payment methods
* Quote VPS deployments
* Create VPS deployments
* Check deployment / order / invoice status
* List and inspect existing VMs
* Power actions
* Rename / reinstall
* Optional per-VM root command execution
* Async command runs, logs, and cancel
* Artifact upload / install flows

Root exec is opt-in per VM.

Example things you can ask your agent:

```
List my Hostodo deployment options.
Quote a 2GB VPS in Detroit with Ubuntu 24.04.
Deploy a VPS named let-test-01 using account credit.
Show me the status of my deployment.
List my Hostodo VMs.
```

---

Offers
------

| Plan | vCPU | RAM | NVMe | Monthly with LETMCP15 | Annual with LETMCP15 |
| --- | --- | --- | --- | --- | --- |
| EPYC-8G3C128GN | 3 | 8GB | 128GB | [$7.65/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-8G3C128GN?promocode=LETMCP15) | [$76.50/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-8G3C128GN?promocode=LETMCP15) |
| EPYC-4G2C64GN | 2 | 4GB | 64GB | [$5.95/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-4G2C64GN?promocode=LETMCP15) | [$59.50/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-4G2C64GN?promocode=LETMCP15) |
| EPYC-2G1C32GN | 2 | 2GB | 32GB | [$2.98/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-2G1C32GN?promocode=LETMCP15) | [$29.75/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-2G1C32GN?promocode=LETMCP15) |
| EPYC-1G1C16GN | 1 | 1GB | 20GB | — | [$17/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-1G1C16GN?promocode=LETMCP15) |

**Promocode**  
`LETMCP15` = 15% off recurring.  
Works in checkout and with MCP / CLI deployment flows. Mention it to the 🤖.

AMD EPYC 7742 · Pure NVMe · 1Gbps · KVM

---

**Network tests:**

Detroit: <https://det01.hostodo.com>  
Las Vegas: <https://lv.hostodo.com>  
Tampa: <https://tpa.hostodo.com>

**OS options include:**

Ubuntu 25.04 / 24.04 / 22.04  
Debian 13 / 12 / 11  
AlmaLinux 9 / 8  
Rocky Linux 9  
CentOS Stream 9  
Fedora 43 / 41  
Arch Linux  
OpenSUSE Leap 15.5  
Alpine

Unmanaged. Instant provisioning. Stripe, PayPal, Crypto, Alipay, and account credit.

Around since 2017.

Helpdesk in <https://console.hostodo.com/>.

* Hassan

---
id: 218750
title: "Announcing Hostodo MCP Server - Control your VPS instances via Claude/Hermes/Codex/Cursor"
date: "2026-07-06T21:20:46+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/218750/announcing-hostodo-mcp-server-control-your-vps-instances-via-claude-hermes-codex-cursor"
---
# Announcing Hostodo MCP Server - Control your VPS instances via Claude/Hermes/Codex/Cursor
**Link:** [Original Thread](https://lowendtalk.com/discussion/218750/announcing-hostodo-mcp-server-control-your-vps-instances-via-claude-hermes-codex-cursor)

Hi LET. We added MCP support for Hostodo.

If you use Claude Desktop, Claude Code, Cursor, Hermes, or another MCP-compatible client, you can now connect it directly to your Hostodo account and manage your VPSes from your AI assistant.

Docs:  
<https://hostodo.com/docs/mcp>

Setup in Console:  
<https://console.hostodo.com/settings/developer-access>

MCP endpoint:

```
https://api.hostodo.com/mcp
```

---

### What it does

The Hostodo MCP server lets your AI client:

* list your VPS instances
* inspect VM details
* start / stop / reboot / reset
* reinstall VMs with a selected OS template
* rename VMs
* run bounded root commands on opted-in VMs
* run longer background commands and poll output
* transfer/install files

WIP: Deploy, helpdesk, etc. Just guaging interest first.

Example prompts:

```
List my Hostodo VMs and show me which ones are online.
```

```
Check disk usage on my production VM.
```

```
Reboot my staging VPS.
```

```
Deploy the docker-compose stack in this directory on my VM.
```

---

### Security model

This is not “paste your SSH key into an AI client.”

Every MCP call is:

* authenticated with a Hostodo developer token
* scoped by permissions like `vms:read`, `vms:power`, `vms:exec`
* checked against VM ownership
* audited
* rate limited

For command execution, there are two gates:

1. the token needs `vms:exec`
2. the VM must have MCP exec explicitly enabled

So you can give an AI client read-only access, power-control access, or exec access depending on what you actually want it to do.

---

### Quick setup

1. Log in to Hostodo Console:  
   <https://console.hostodo.com>
2. Go to Settings → Developer Access:  
   <https://console.hostodo.com/settings/developer-access>
3. Create a token with the scopes you want.
4. Add the MCP server to your client.

Claude Code example:

```
claude mcp add --transport http \
  --header "Authorization: Bearer <your-token>" \
  hostodo https://api.hostodo.com/mcp
```

Hermes example:

```
hermes mcp add hostodo --url https://api.hostodo.com/mcp --auth header
```

Full docs:  
<https://hostodo.com/docs/mcp>

---

### LETMCP15

For LET users testing the MCP beta:

`LETMCP15` = 15% off recurring

Works at checkout on Hostodo Console.

AMD EPYC 7742 · Pure NVMe · 1Gbps · KVM

| Plan | vCPU | RAM | NVMe | Monthly with LETMCP15 | Annual with LETMCP15 |
| --- | --- | --- | --- | --- | --- |
| EPYC-1G1C16GN | 1 | 1GB | 20GB | — | [$17/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-1G1C16GN?promocode=LETMCP15) |
| EPYC-2G1C32GN | 2 | 2GB | 32GB | [$2.98/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-2G1C32GN?promocode=LETMCP15) | [$29.75/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-2G1C32GN?promocode=LETMCP15) |
| EPYC-4G2C64GN | 2 | 4GB | 64GB | [$5.95/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-4G2C64GN?promocode=LETMCP15) | [$59.50/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-4G2C64GN?promocode=LETMCP15) |
| EPYC-8G3C128GN | 3 | 8GB | 128GB | [$7.65/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-8G3C128GN?promocode=LETMCP15) | [$76.50/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-8G3C128GN?promocode=LETMCP15) |
| EPYC-16G6C192GN | 6 | 16GB | 192GB | [$17/mo](https://console.hostodo.com/instances/deploy/TPA01/EPYC-16G6C192GN?promocode=LETMCP15) | [$170/yr](https://console.hostodo.com/instances/deploy/TPA01/EPYC-16G6C192GN?promocode=LETMCP15) |

Prices above are verified against the Hostodo production quote engine.

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
Fedora 43 / 41  
Arch Linux  
OpenSUSE Leap 15.5  
And more.

---

Unmanaged. Instant provisioning. Stripe, PayPal, Crypto, and Alipay.

Around since 2017. Same Hostodo, better everything.

Feedback welcome here, especially if you try the MCP integration with Claude/Cursor/Hermes/etc.

Questions here via helpdesk.

* Hassan

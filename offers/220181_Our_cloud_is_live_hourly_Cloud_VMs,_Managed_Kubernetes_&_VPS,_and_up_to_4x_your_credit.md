---
id: 220181
title: "Our cloud is live: hourly Cloud VMs, Managed Kubernetes & VPS, and up to 4x your credit"
date: "2026-08-15T14:32:33+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/220181/our-cloud-is-live-hourly-cloud-vms-managed-kubernetes-vps-and-up-to-4x-your-credit"
---
# Our cloud is live: hourly Cloud VMs, Managed Kubernetes & VPS, and up to 4x your credit
**Link:** [Original Thread](https://lowendtalk.com/discussion/220181/our-cloud-is-live-hourly-cloud-vms-managed-kubernetes-vps-and-up-to-4x-your-credit)

☁️ Our cloud is live: hourly Cloud VMs & Managed Kubernetes, and up to 4x your credit
-------------------------------------------------------------------------------------

Hey LET 👋

RareCloud started on this forum, and this community is what grew it. So for the biggest thing we have ever shipped, we brought it back home. Over the past year we tore the old thing down and rebuilt pretty much everything: a new in-house console, our own cloud, and the automation stack around it.

And we did not come home empty-handed. Together with **LowEndBox** we lined up a welcome for this community: a launch offer that can **double, triple, even quadruple** your credit. More on that below.

> If you want the outside view first, LowEndBox wrote the whole thing up here:  
> 👉 **[RareCloud Returns to LowEndBox, With a Rebuilt Cloud Platform, New Console, Kubernetes, MCP, and Up to 4x Credit](https://lowendbox.com/blog/rarecloud-returns-to-lowendbox-with-a-rebuilt-cloud-platform-new-console-kubernetes-mcp-and-up-to-4x-credit/)**

---

### What you can spin up now

We built you a brand-new dashboard from the ground up, the [**Console**](https://console.rarecloud.io/ "**Console**"): one login and one balance for everything you run with us. Here is what you can actually do with it:

* **Cloud VMs from €3.99/month**, from click to SSH in **under a minute**. Billed by the hour and capped at the monthly price: a test box you kill after two hours costs two hours, a box you run flat-out all month never goes past the cap. Cost-optimized and general-purpose plans on shared vCPU for everyday web and apps; CPU- and memory-optimized plans on dedicated vCPU for build farms, databases and heavy jobs.
* **Managed Kubernetes with a free control plane**: you pay only for the worker nodes. Point `kubectl` at it and ship, autoscale the pool when traffic spikes and scale it back down after, so you run production Kubernetes without babysitting the cluster or paying to keep it alive.
* Put it together: attach **Block Storage**, drop a **Load Balancer** in front, sit it on a **private network** with **reserved IPs and firewalls**, all managed for you and ready the moment your project needs to grow.
* Traffic is **included** on every plan, overage is a flat **€1/TB** with no surprise egress bills, and every invoice carries **EU VAT**.

And your existing **KVM VPS, dedicated servers, hosting and proxies are all still here, still running, untouched**, on the same login and the same balance. Bucharest is the first full cloud region, with more of our locations becoming real cloud regions over time.

---

### Built for code, and for AI agents

This is the part we built for the LET crowd. The **public REST API is the source of truth**, and every other tool is just a client of it: a **Go CLI**, a **Terraform provider** to manage RareCloud as code, and an **MCP server** so you can hand Claude, Cursor or any MCP client a scoped token and let it work. Create, resize, power, reinstall, add SSH keys, attach volumes, reserved IPs and firewalls, across Cloud VMs, Kubernetes and legacy VPS alike.

**Drive your infrastructure by hand, by pipeline, or by prompt.**

Here is how LowEndBox put it, unprompted:

> "RareCloud appears to have gone all in on building its own platform ... a much more cloud-native feel than a typical VPS provider, while still keeping its existing hosting products under the same account."
>
> "The company says the API is the source of truth, with the web console simply acting as another client. And that's the right way to build."

---

### 🎁 The offer: up to 4x credit (RareCloud × LowEndBox)

RareCloud started on LowEndTalk, so our most generous credit offer ever lands here first. Add funds, and we multiply them:

* Top up **any amount** and it is **doubled**.
* Top up **€25 or more** and it is **tripled**.
* Top up **€100 or more** and it is **quadrupled**.

One boosted top-up per account, applied **automatically** the moment you pay, **no code to enter.** The bonus spends everywhere: hourly cloud, brand-new orders, even renewals of the VPS, hosting and proxies you already run.

**The math:**

| You add | You get |  |
| --- | --- | --- |
| €25 | **€75** | 3x |
| **€100** | **€400** | **4x, best value** |
| €1,000 | **€4,000** | 4x |

Our prices already sit among the lowest you will find for what you get. The quadruple takes them to a quarter of list. Real examples at current prices:

**KVM VPS (yearly, list vs 4x):**

| Plan | Specs | Normal /year | With 4x credit |
| --- | --- | --- | --- |
| Starter KVM | 1 vCPU · 1 GB · 3 TB | €29.50 | **€7.38** |
| Core VPS | 1 vCPU · 2 GB · 3 TB | €45.00 | **€11.25** |
| Plus VPS | 2 vCPU · 4 GB · 5 TB | €95.00 | **€23.75** |
| Pro VPS | 4 vCPU · 8 GB · 7 TB | €195.00 | **€48.75** |
| Elite VPS | 4 vCPU · 16 GB · 10 TB | €345.00 | **€86.25** |

**Cloud VMs (monthly, billed hourly and capped at the monthly price):**

| Plan | Specs | Normal /month | With 4x credit |
| --- | --- | --- | --- |
| S-1 | 1 vCPU · 2 GB · 1 TB | €3.99 | **€1.00** |
| S-2 | 2 vCPU · 4 GB · 2 TB | €6.99 | **€1.75** |
| G-1 | 1 vCPU · 4 GB · 4 TB | €7.99 | **€2.00** |
| G-2 | 2 vCPU · 8 GB · 6 TB | €14.99 | **€3.75** |
| G-4 | 4 vCPU · 16 GB · 8 TB | €27.99 | **€7.00** |

Same story on the doubled and tripled tiers, and the bonus spends on renewals too, so it stretches what you already run with us.

➡️ **Claim it here: [console.rarecloud.io/billing/credit/add](https://console.rarecloud.io/billing/credit/add)**  
Offer runs until **August 31**.

---

### 🌍 Where it runs

12 locations across three continents, one login and one balance covering all of it:

* **Cloud:** 🇷🇴 Bucharest, our first cloud region, with more of our locations becoming cloud regions over time
* **Dedicated servers:** 🇷🇴 Timișoara
* **VPS:** 🇷🇴 Constanța · 🇩🇪 Germany · 🇳🇱 The Hague · 🇬🇧 London · 🇺🇸 New York, Silicon Valley, Phoenix, Dallas · 🇭🇰 Hong Kong · 🇯🇵 Tokyo

---

### 🚀 Why RareCloud

* A real cloud you can **script end to end**: Cloud VMs, Managed Kubernetes, block storage, load balancers and private networking, all from one API
* Cloud VMs **billed by the hour with a monthly cap**, a busy month never turns into a surprise bill
* **API-first**: REST API + Go CLI + Terraform + MCP, scoped tokens you control
* Your existing **VPS, dedicated, hosting and proxies stay exactly as they are**, one login, one balance
* Transparent pricing, traffic included, **EU VAT invoices your accountant can actually book**
* And right now, **up to 4x on your credit** to try all of it, until Aug 31

**Payments:** card (Stripe), crypto (CoinGate), PayPal, Alipay, bank transfer.

---

### 💶 €500 in free credits: you write our roadmap

> **Every useful idea in this thread is eligible.** No forms, no "share it on three platforms", no account needed. Tell us what to build next, and the best calls get paid in credit.

We shipped the cloud, but the roadmap from here is yours to shape. We would rather spend €500 finding out what you actually want us to add than guess it in a meeting.

**Here is what we are already lining up:**

* **AI Sandboxes** in the cloud: secure, isolated environments to run untrusted or AI-generated code
* **S3-compatible object storage**
* **A container registry**
* **One-click templates** to deploy the apps you actually use, the trending ones and the essentials, in a couple of clicks

**Now tell us what to build.** When the campaign closes we read **every single comment** and pay out for the ideas that shape what we ship next, in four sizes until the whole pool is gone:

| Bonus | What earns it |
| --- | --- |
| **€100** | The idea that changes what we build next. Someone will get this. |
| **€50** | A feature or service we had not planned, with a real use case behind it. |
| **€20** | A concrete, specific request, the kind we can put straight on the board. |
| **€10** | Any genuinely useful suggestion. Yes, including a good one-liner. |

**€500 total, and we keep awarding until it is gone.** However many ideas deserve credit, that is how many get it.

**What we want to hear:**

1. **Which of the four above should we ship first?**
2. **What is not on that list that you need us to add?** A service, a feature, a location, a template.
3. **What one thing, if we built it, would move more of your stack to us?**

**Ground rules:**

* **Specific wins.** "Add X, because it would let me do Y" beats "more features please".
* **Dream big or dream small.** A whole new service and a one-line quality-of-life fix both count.
* **Haters' comments will be ignored.** Constructive only: tell us what to build, not just what you dislike.

**The boring but important bits.** The campaign runs until **August 31**, the same deadline as the credit offer. Winners are picked once it closes, announced in this thread and contacted directly. The credit lands on your account, new or existing, and there is nothing to buy: you do not even need to be a customer to comment. Judged by us on usefulness alone, not a lottery and not a popularity contest.

**So tell us what to build next.** 👇

---

We are not the same RareCloud from a year ago. Come kick the tyres, weigh the pricing against what you run today, and if you hit a bug, say so in the comments. We will be in the thread.

Cheers,  
**The RareCloud Team**

---

**Offer terms:** add funds through August 31, 2026. Any single top-up is doubled (2x total); €25 or more is tripled (3x total); €100 or more is quadrupled (4x total). One promotional grant per account, applied automatically to your first qualifying top-up (€5 to €5,000 per top-up; amounts counted at their EUR value). Bonus credit is valid for 60 days from the top-up and is spent before your regular balance. RareCloud may end or amend this offer before the deadline.

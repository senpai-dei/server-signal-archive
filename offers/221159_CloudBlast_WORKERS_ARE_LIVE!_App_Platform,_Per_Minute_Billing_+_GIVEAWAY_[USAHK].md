---
id: 221159
title: "CloudBlast WORKERS ARE LIVE! App Platform, Per Minute Billing + GIVEAWAY [USA/HK]"
date: "2026-09-18T17:02:24+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/221159/cloudblast-workers-are-live-app-platform-per-minute-billing-giveaway-usa-hk"
---
# CloudBlast WORKERS ARE LIVE! App Platform, Per Minute Billing + GIVEAWAY [USA/HK]
**Link:** [Original Thread](https://lowendtalk.com/discussion/221159/cloudblast-workers-are-live-app-platform-per-minute-billing-giveaway-usa-hk)

![](https://i.imgur.com/28qE40P.png)

🚀 INTRODUCING CLOUDBLAST WORKERS 🚀
==================================

### ⚡ Git Push to Live URL | Per Minute Metering | 100+ Templates | Salt Lake City / Hong Kong (UK Coming Soon)

Hello LowEndTalk Community! 👋

You already know us for hourly billed AMD EPYC VPS. Today we are launching something new: **Workers**, our app platform.

Think Railway, Render, Fly.io or Vercel, but priced the way LET expects things to be priced. Point us at a Git repository, a Docker image or one of our templates, pick a datacenter, and your app is online with a public URL and SSL. No Dockerfile required, no pipeline to write, no server for you to patch or babysit.

**Deploy now:** <https://console.cloudblast.io/>  
**Product page:** <https://cloudblast.io/workers>

---

🎉 LAUNCH GIVEAWAY: 10€ FREE CREDIT
----------------------------------

To celebrate the launch we are giving **10€ of account credit** to one lucky LET member.

### 👉 How to enter

Just comment:  
`BLAST ME`

One winner is picked at random and announced **30 days after this thread was posted**. The credit works on Workers, on our VPS, or on both.

---

🧩 WHAT IS A WORKER?
-------------------

A worker is an application, service or database that we build and run for you in an isolated container. You give it a repo, an image or a template, choose the region and the resources it may use, and it goes live. You never touch a server.

* 🛠️ **Any language, any framework**  
  Node, Python, Go, Rust, PHP, Ruby and more, or bring your own Dockerfile.
* 🤖 **Zero configuration**  
  We detect the build, install the dependencies and start the process for you.
* ⏪ **One click back to a working version**  
  Every deploy is kept, so a bad release is undone in seconds.
* 💾 **Persistent disks**  
  Attach a disk to any worker and it survives redeploys, restarts and scaling. Postgres, MySQL, Redis and MongoDB all work.
* 📈 **Logs, metrics and SSL included**

Nothing extra to bolt on, nothing extra to pay for.
---------------------------------------------------

🔁 HOW IT WORKS
--------------

1. **Connect** a Git repository, a Docker image or one of the 100+ templates.
2. **Build** happens automatically on every push, with instant rollback to any earlier version.

3. **Run** with a public URL, SSL, logs, metrics and a persistent disk if it needs one.
---------------------------------------------------------------------------------------

💶 PRICING: FOUR METERS, NOTHING ELSE
------------------------------------

No plans to choose, no seats to buy, no minimum to clear. **Usage is measured per minute** and only while the worker runs, then charged at the hourly rates below. Stop a worker and the CPU and RAM meters stop with it. Run something for 8 minutes and you pay for 8 minutes, not for a full hour.

| Meter | Price | Unit |
| --- | --- | --- |
| CPU | €0.011 | per core hour |
| RAM | €0.004 | per GB hour |
| Disk | €0.0001 | per GB hour |
| Traffic | €0.01 | per GB out |

Measured per minute, charged at the hourly rates above, invoiced once a month. **1 vCPU + 2 GB RAM running the full month lands at roughly 14€.**

---

📊 THE SAME WORKLOAD, A FRACTION OF THE BILL
-------------------------------------------

One vCPU and 2 GB of RAM, for the hundred hours a month that a scheduled job or a staging environment actually runs:

|  | **CloudBlast** | Fly.io | Railway | Vercel |
| --- | --- | --- | --- | --- |
| vCPU, per hour | **€0.0110** | n/a | €0.0252 | €0.1178 |
| RAM, per GB hour | **€0.0040** | €0.0063 | €0.0126 | €0.0098 |
| Outgoing traffic, per GB | **€0.01** | €0.02 | €0.05 | €0.14 |
| Minimum monthly fee | **none** | none | €4.60 | €18.40 |
| **1 vCPU + 2 GB, 100 hrs/month** | **€1.90** | €4.06 | €5.04 | €18.40 |
|  |  | 2.1x | 2.7x | 9.7x |

*Public list prices taken from each provider's own pricing page in September 2026 and converted from US dollars at $1 = €0.92. The monthly figure is what the workload actually costs: the cheapest plan that allows it, plus any usage the plan's included credit does not cover. "n/a" means the resource is not sold by the unit, only inside a fixed machine size or plan.*

---

📦 100+ TEMPLATES, ONE CLICK AWAY
--------------------------------

Frameworks, databases, queues, dashboards and automation tools, already configured. Pick one, name it, deploy.

**Frameworks:** Next.js, Nuxt, Node.js, Express, NestJS, Astro, Remix, SvelteKit, Django, FastAPI, Flask, Laravel, Ruby on Rails, Spring Boot, Go, Rust, Deno, Bun, PHP, Python

**Data:** PostgreSQL, MySQL, MariaDB, MongoDB, Redis, ClickHouse, Elasticsearch, Meilisearch, MinIO, RabbitMQ, Supabase, PocketBase

**Apps and tooling:** WordPress, Ghost, Strapi, Directus, n8n, Grafana, Prometheus, Metabase, Plausible, Umami, Gitea, Mattermost, Nextcloud, Ollama, Discord and Telegram bots

...and 250+ more.

![](https://i.imgur.com/20nlkTE.png)

🗺️ WHERE WORKERS RUN
--------------------

Two regions at launch, one more on the way. You pick the region per worker.

| Location | Status | Looking glass IPv4 | Looking glass IPv6 |
| --- | --- | --- | --- |
| Salt Lake City, USA | Live | 192.166.82.235 | 2a13:9500:3f:d7::0 |
| Hong Kong | Live | 178.83.121.94 | 2a0e:97c0:181:59::0 |
| Birmingham, UK | Coming soon | n/a | n/a |

Live latency tests and download files for each region: <https://cloudblast.io/workers>

---

🔄 MOVING OVER FROM RAILWAY, RENDER, FLY.IO OR VERCEL?
-----------------------------------------------------

In most cases you will not need to change any code. Connect the same repository or Docker image, set the environment variables, attach a disk if you need one, and switch your domain over. If something does not fit, our support is available 24/7 and we will look at it with you.

---

💳 PAYMENT METHODS
-----------------

Cryptocurrencies (XMR included), credit cards, Alipay, WeChat Pay and 20+ local payment methods.

First time signing up, a 10€ deposit is required to start deploying. After that any amount works with usage based billing.

---

❓ QUICK FAQ
-----------

**Is there a plan, a seat fee or a minimum?**  
No. No plans, no per user seats, no minimum spend. You pay for the resources your workers use and nothing else.

**Can I run a database?**  
Yes. Attach a persistent disk and it survives redeploys, restarts and scaling.

**How granular is the billing?**  
Usage is measured per minute and charged at the hourly rates. A worker that ran for 20 minutes costs a third of an hour, not a full one. Invoices go out monthly.

**What happens when I stop a worker?**  
The CPU and RAM meters stop with it. Disk keeps metering while the data is kept.

**Do I need a Dockerfile?**  
No, but you can bring one if you prefer it.

---

### [👉 DEPLOY YOUR FIRST WORKER: console.cloudblast.io](https://console.cloudblast.io/)

Questions, feature requests or a repo that will not build? Post here and we will answer, or join our Discord: <https://discord.gg/7M84Xp8QBr>

Happy deploying! 🚀

---
id: 221289
title: "ServersCamp: Database-Tuned Cloud | €25 Free Test Credit"
date: "2026-09-21T14:01:44+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/221289/serverscamp-database-tuned-cloud-25-free-test-credit"
---
# ServersCamp: Database-Tuned Cloud | €25 Free Test Credit
**Link:** [Original Thread](https://lowendtalk.com/discussion/221289/serverscamp-database-tuned-cloud-25-free-test-credit)

Hi LET,

My name is Oleksandr and I am the founder of ServersCamp.  
We are building a cloud provider, [https://serverscamp.com](https://serverscamp.com/?utm_source=lowendtalk&utm_medium=forum&utm_campaign=testers)

### What is it?

We are trying to tune our cloud for databases, and naturally it works great for other workloads too.  
To get there we had to do a lot of custom stuff, both in solutions and in architecture.  
Also took a lot from the enterprise world.  
In theory the whole set should look like this, this is what every VM technically gets:

### 1. Hardware

We already have 2 types of hardware, old first gen Xeon Scalable and latest EPYC.  
No middle ground yet, planning to add Genoa or Milan.

### 2. Network

No real alternatives here, so Mellanox cards and Mellanox switches, with RDMA, eBGP, PFC.  
Software side is OVN.

### 3. Disks

No local disks at all. What good are they if the node physically goes down.  
All storage is SDS, replicated network storage on NVMe disks, default replica 2 for now.  
Synthetics showed great results, around 150-160 us qd1.

### 4. Backups

Here we got inspired by enterprise and went the DR backups way.  
Our backup supports multi backend, at the moment the backends are: our S3 (same DC, but outside of SDS), Wasabi and Impossible Cloud.  
We also added encryption, possibility to download from the backends and automatic checks that the backup is alive at all.  
Meaning, after every backup, besides md5 it also gets physically downloaded and boot is started, we check if the VM was able to start from that backup.

### 5. Security

We tried, and it seems we succeeded, to integrate Suricata in a way that you can build zero trust even in a flat network.  
Beyond firewall rules, we wanted visibility into what's actually happening in the traffic, with the option to block threats inline. For every VM you can enable inline, it stays transparent for everyone, but traffic analysis and interception happens on the underlay network level. Not all functionality works yet.

### 6. Redundancy and geo

Right now we have one site in Bucharest, Romania, EU.  
We don't want to stop at one, so we already made a deal with another provider and are working on the second site. It will give us another location, very good international peering and serious anti-DDoS protection.

=========================================================

Here are our tests:  
<https://serverscamp.com/docs/benchmarks/block-storage-vs-local-nvme>  
<https://serverscamp.com/docs/benchmarks/hetzner-vs-serverscamp-postgres>

Third party:  
<https://serververify.com/benchmarks/5c644141-aa29-488a-ae48-bd646d3b07b5>  
<https://www.vpsbenchmarks.com/yabs/serverscamp-12c-63gb-20260724-f759f0>

=========================================================

It works already.  
But our tests are one thing, how the platform behaves under live load is another, and we want to see it.  
So we invite anyone interested to come and test our cloud.  
We prepared capacity for this on nodes of different generations.

1. Total slots 50-100. Depends on the load and how much the cluster can take without overall degradation.
2. Max instance size 2 cores and 4 GB RAM + 100 GB disk.
3. Please don't use it for abuse, miners and such.
4. Please don't create multi accounts.

### How to start

1. Register at [https://serverscamp.com](https://serverscamp.com/?utm_source=lowendtalk&utm_medium=forum&utm_campaign=testers) and confirm your email.
2. Open a ticket mentioning LET or PM me here. We will set up your account manually and add 25 euro of credit for 1 month.  
   Account setup currently needs a card. For LET we do it manually, so you don't need to add one. Until we do the setup, you won't be able to create anything.

We will be adding redeem codes here from time to time and posting updates.  
And if you need more, just open a ticket.

Really want to get feedback. Thanks. ![:)](https://lowendtalk.com/resources/emoji/smile.png ":)")

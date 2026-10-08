---
id: 221853
title: "CubePath Object Storage: S3 compatible, 5 GB free every month, $9/TB after"
date: "2026-10-08T03:18:06+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/221853/cubepath-object-storage-s3-compatible-5-gb-free-every-month-9-tb-after"
---
# CubePath Object Storage: S3 compatible, 5 GB free every month, $9/TB after
**Link:** [Original Thread](https://lowendtalk.com/discussion/221853/cubepath-object-storage-s3-compatible-5-gb-free-every-month-9-tb-after)

CubePath Object Storage: S3 compatible, 5 GB free every month, $9/TB after
--------------------------------------------------------------------------

Hi LET,

We've just launched our own **S3 compatible Object Storage**, running on our own hardware in **Barcelona, Spain (EU)**. Every account gets a free tier each month, with no trial period and no expiry.

### Free every month

* **5 GB** storage
* **5 GB** egress
* **20,000** requests
* **1,000,000** event notification deliveries

### After the free tier

|  | Price |
| --- | --- |
| Storage | ~$9 per TB/month ($0.0088/GB) |
| Egress | ~$10 per TB ($0.0098/GB) |
| Class A requests (PUT, LIST...) | $0.006 per 1,000 |
| Class B requests (GET, HEAD...) | $0.0006 per 1,000 |

No minimum, billed hourly on what you actually store.

### Features

* Fully S3 compatible: works with AWS CLI, rclone, restic, boto3, any S3 SDK
* Versioning and Object Lock (governance and compliance)
* Lifecycle rules
* Encryption at rest (SSE-S3, on by default)
* Replication to another CubePath bucket or any external S3 bucket
* Bucket event notifications to webhooks
* Read only or read/write access keys
* Native integration with the CubePath CDN for public delivery
* Built-in file browser in the dashboard, plus API, CLI (`cubecli`) and MCP for AI assistants

The current tier is **Infrequent Access**, which is a good fit for backups, archives, media and offsite copies. An SSD Standard tier is coming later.

### Get started

* Product page and pricing: [cubepath.com/object-storage](https://cubepath.com/object-storage)
* Already a customer? Create your first bucket at [my.cubepath.com/object-storage](https://my.cubepath.com/object-storage)

We'd love your feedback, and we're happy to answer any questions here.

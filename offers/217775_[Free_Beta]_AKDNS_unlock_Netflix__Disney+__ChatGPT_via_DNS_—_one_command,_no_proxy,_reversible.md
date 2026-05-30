---
id: 217775
title: "[Free Beta] AKDNS: unlock Netflix / Disney+ / ChatGPT via DNS — one command, no proxy, reversible"
date: "2026-05-30T20:07:20+00:00"
author: "Unknown"
link: "https://lowendtalk.com/discussion/217775/free-beta-akdns-unlock-netflix-disney-chatgpt-via-dns-one-command-no-proxy-reversible"
---
# [Free Beta] AKDNS: unlock Netflix / Disney+ / ChatGPT via DNS — one command, no proxy, reversible
**Link:** [Original Thread](https://lowendtalk.com/discussion/217775/free-beta-akdns-unlock-netflix-disney-chatgpt-via-dns-one-command-no-proxy-reversible)

Hi LET,

We've been building **AKDNS** over at Akile and it's now in open beta — figured this crowd would actually get the point of it. It's a **DNS-based unlock / routing** service: point a box's resolver at AKDNS and it steers streaming and AI domains to unlock-capable nodes. No proxy client, no tunnel, and it leaves the rest of your traffic alone.

There's a **free tier**, so you can just try it on a spare box without committing to anything.

**How it works**

Routing happens at the DNS layer. When your server resolves, say, `netflix.com`, AKDNS hands back an unlock node in the matching region so that request egresses over a route that can unlock the service. Anything you haven't configured resolves normally and stays direct — so there's essentially no added latency on everything else, and nothing is proxied. Rules are per-IP, so each box is configured independently.

**Free / pricing**

* Open beta, free right now.
* Sign in with an AKILE account (OAuth) → AKILE IPs are unlimited.
* Not on AKILE? You can still add **10 IPs for free**.

**Locations (multi-region BGP)**

Hong Kong, Japan, US, Singapore, Korea, Taiwan, Germany, UK. The setup script speed-tests them and picks the best one for you automatically.

**Supported services (60+)**

* Streaming: Netflix, Disney+, HBO Max, YouTube, Prime Video, Hulu, Paramount+, HotStar, DAZN…
* AI: ChatGPT, Claude, Gemini, Sora, Copilot, Meta AI
* JP / TW / HK local: ABEMA, U-NEXT, TVer, Bahamut Anime (动画疯), KKTV, MyTVSuper, ViuTV…
* Plus TikTok, Instagram, Reddit, Spotify, etc.

**Setup**

One command on a Linux box as root/sudo, drops you into an interactive menu:

```
wget -qO- https://raw.githubusercontent.com/akile-network/aktools/refs/heads/main/akdns.sh | bash
```

Rough flow: add the IP in the console → run the unlock baseline test → DNS speed test → set as system DNS → tick the services to unlock for that IP → re-test. (The two middle steps have a combined "speed-test & set" option in the menu.)

If `wget | bash` makes you pause — good instinct. The script is public at `akile-network/aktools`, so read it before you run it.

**The "set as system DNS" part — being upfront**

This is LET, so I'll spell it out: that option doesn't just append a nameserver. To make sure lookups actually hit AKDNS regardless of your distro's resolver, it disables whatever is managing DNS (systemd-resolved / NetworkManager / resolvconf / netplan), writes a static `/etc/resolv.conf` pointed at the best node, and `chattr +i` locks it so dhclient / cloud-init can't clobber it on reboot.

It backs everything up before touching anything, and "Restore DNS config" reverts the whole thing — unlocks the file, re-enables your original manager, puts you back where you were. The script only does connectivity checks + DNS config; it doesn't install a proxy and doesn't alter your traffic.

**Links**

* Site / console: <https://dns.akile.ai>
* Docs: <https://dns.akile.ai/docs>
* Telegram (feedback / request a service): <https://t.me/+MEKKEBUkW6ZjMzBl>

It's beta — if something won't unlock or you want a service added, the TG group is the fastest line to us and turnaround is quick. Feedback welcome, including the critical kind.

*(Disclosure: drafted with AI; let me know if anything reads wrong and I'll fix it.)*

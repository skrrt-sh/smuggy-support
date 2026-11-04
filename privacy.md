---
layout: page
title: Privacy policy
permalink: /privacy/
description: What Smuggy contacts, what it keeps on your Mac, and how to delete it. Smuggy collects no personal data.
---

# Privacy Policy

Effective 2026-11-04.

Smuggy collects no personal data. It has no accounts, no analytics, no crash reporting and no
tracking, and it never sends anything to its developers.

## Your traffic

- **DPI Bypass** reshapes your traffic on your Mac and sends it straight to the site you are
  visiting. Nothing is tunnelled.
- **VPN** sends your traffic to the servers you add, or straight to the sites your routing rules
  keep direct. Those servers are run by you or your provider, not by Smuggy, and their own
  policies apply.

## What Smuggy contacts on its own

- **Cloudflare's connectivity check**, `cp.cloudflare.com`, requested through each of your VPN
  servers to measure its delay and learn which country its traffic exits from: when you test your
  servers, once a minute while Servers, or Home in VPN mode, is on screen, and every one to five
  minutes while the VPN is on, through every server whichever you picked, so automatic selection
  can pick the fastest. For an AmneziaWG server the check is a lookup
  of that name through the server. Cloudflare sees the server's exit address, not yours.
- **Your VPN servers directly**, with a plain TCP handshake to each, to time them when the
  connectivity check can't run.
- **DNS servers.** In VPN mode, lookups go through your VPN to the resolvers in Routing › DNS
  (1.1.1.1 and 8.8.8.8 unless you change them). Lookups outside the VPN, in DPI Bypass, for names
  your rules keep direct and for your servers' own names, go to the resolvers you set for direct
  traffic or, by default, your network's. If your network names none, Smuggy uses Cloudflare's
  1.1.1.1 and Google's 8.8.8.8; the version downloaded from GitHub asks them alongside your
  network's resolvers every time.
- **Subscription links you add**, fetched when you add them and, while automatic updates are on,
  again on their schedule: daily unless you or your provider change it, and at launch if you turn
  that on. Each fetch goes directly or through your VPN, as you choose. It names Smuggy as another
  app in its User-Agent, v2rayN unless you pick another, because providers choose the format they
  send by it. It also sends any headers you add, and device headers only if you turn them on: a
  random ID made on your Mac, your macOS version and your Mac's model, which let a provider count
  your devices.
- **Routing you add from a link**, downloaded again from that link on the same schedule.
- **Rule lists you install**, downloaded from their projects' releases on GitHub and checked
  against the checksums published there, then updated daily or weekly. A list you import from a
  link is downloaded from it once.
- **Update checks**, in the version downloaded from GitHub only: it asks GitHub once a day whether
  a newer version is out, and downloads it from there.

## What Smuggy contacts when you ask

- **Cloudflare's speed test**, `speed.cloudflare.com`, through the server you measure: 10 MB down
  and up to 8 MB up.
- **Sites you ask the strategy finder to test**, and your network's resolvers to look them up, to
  find a strategy that reaches them.
- **Smuggy's website, `smuggy.skrrt.sh`, in your browser**, for Help and Support.
- **GitHub, in your browser**, for Report a problem. It fills in a public issue in
  `skrrt-sh/smuggy-support` with your Smuggy
  and macOS versions and how Smuggy is set up, naming no sites, servers or keys. Nothing is sent
  unless you submit it.

## What stays on your Mac

Your settings, strategies, servers and their keys, subscriptions with their links, headers and
device ID, routing rules, including those adaptive strategies save for sites, lists, the Wi-Fi
names you save, and Smuggy's logs are stored only on your Mac. None of it is uploaded anywhere.
macOS shows Wi-Fi names only to apps with Location access, so Smuggy asks for it only when you save
a Wi-Fi network; it never records where you are. Export your data writes your strategies, servers,
subscriptions, routing, lists and networks to a file you choose, and can leave out keys and
passwords, subscription links and headers, the device ID and Wi-Fi names.

## Retention and deletion

Smuggy collects nothing, so there is nothing to ask us to delete. What it stores on your Mac stays
until you remove it: delete servers, subscriptions, rules, lists or networks in the app, reset
them in Settings › Privacy & Data, or remove Smuggy and its data. That data is in
`~/Library/Containers/com.skrrt.smuggy`, Smuggy's folder in `~/Library/Group Containers` and
Smuggy's entry in your keychain, or, for the version downloaded from GitHub,
`~/Library/Application Support/Smuggy`, `~/Library/Preferences/com.skrrt.smuggy.plist` and the
network helper's log in `/Library/Logs/Smuggy`.

## Third parties

Smuggy does not sell, use, or disclose to third parties any user data for any purpose.

## Changes and contact

If this policy changes materially, Smuggy shows its privacy notice again before you next use it. Questions go to [support@skrrt.sh](mailto:support@skrrt.sh), or see
[Smuggy support](https://smuggy.skrrt.sh/support/).

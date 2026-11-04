---
layout: page
title: Support
permalink: /support/
description: How to start with Smuggy, answers to common questions, and how to reach the people who make it.
---

# Smuggy support

How to start, answers to common questions, and how to reach the people who make Smuggy.

## Contact us

Email [support@skrrt.sh](mailto:support@skrrt.sh). Tell us your Smuggy version, from Settings ›
About, your macOS version, which mode you use and what you expected to happen. Leave out server
links and keys: we never need them.

Found a bug? **Report a Problem**, in the toolbar of Smuggy's window or in Settings › Diagnostics, opens a
[GitHub issue](https://github.com/skrrt-sh/smuggy-support/issues) already filled in with how Smuggy
is set up, naming no sites, servers or keys.

Skrrt LLC makes Smuggy.

## Getting started

1. Open Smuggy from the menu bar.
2. Pick a mode at the top of the window or the popover: **DPI Bypass** or **VPN**.
3. Click the power button. The first time, macOS asks to add a VPN configuration for Smuggy. Allow
   it: Smuggy carries every app's traffic through that configuration, in both modes.

DPI Bypass needs nothing else. VPN mode needs a server: click **Add** and paste a share link, a
subscription link or an Amnezia key from your provider.

## Common questions

<details markdown="1">
<summary>Why does Smuggy add a VPN configuration if I only use DPI Bypass?</summary>

That is how macOS lets an app handle traffic from every other app. In DPI Bypass mode the
configuration connects to no server: Smuggy reshapes your traffic on your Mac and sends it straight
to the site over your own connection.

</details>

<details markdown="1">
<summary>Does Smuggy come with VPN servers?</summary>

No. Smuggy does not sell or provide VPN service. VPN mode works with servers you run or get from a
provider: VLESS, VMess, Trojan, Shadowsocks, Hysteria 2, WireGuard and AmneziaWG. DPI Bypass needs
no server at all.

</details>

<details markdown="1">
<summary>Smuggy is on, but a site still doesn't load</summary>

- Turn on **Adaptive strategies** in Settings › Connection. When a site doesn't load, Smuggy tries
  its other strategies and remembers the one that works there.
- On the Strategies page, click **Find for My Sites** and name the site. Smuggy tries other
  strategies on it and keeps the one that reaches it. Turn off VPN mode first, or the tests only
  show what the VPN reaches.
- If none does, the site can't be reached by reshaping packets alone; VPN mode can reach it through
  your server.

</details>

<details markdown="1">
<summary>Is my traffic sent to Skrrt?</summary>

No. Smuggy has no accounts, analytics or tracking, and it never sends anything to us. The
[privacy policy](/privacy/) lists everything Smuggy contacts and stores.

</details>

<details markdown="1">
<summary>What does the kill switch do?</summary>

In VPN mode, if the tunnel drops, the kill switch stops traffic instead of letting it go out
unprotected. It's on from the start; you can turn it off in Settings › Connection.

</details>

<details markdown="1">
<summary>How do I start over or remove my data?</summary>

Settings › Privacy & Data › Reset puts one area, or everything, back to how it was on first launch.
The [privacy policy](/privacy/#retention-and-deletion) lists where Smuggy keeps its data on your
Mac, if you want to remove it after deleting the app.

</details>

<details markdown="1">
<summary>How do I get a refund?</summary>

Purchases from the Mac App Store are refunded by Apple. Request one at
[reportaproblem.apple.com](https://reportaproblem.apple.com).

</details>

## Requirements

Smuggy needs macOS 26 or later, on a Mac with Apple silicon or Intel.

---
title: "Kali Desktop Experience for WSL"
weight: 1
tags: ["Linux", "Kali-Linux", "WSL"]
categories: ["Notes"]
date: 2020-08-19
draft: false
author: "Prajwal"
authorLink: "https://prajwalyashasvi.in"
timeToRead: "8"
featured: true
---

Kali Linux is giving its Windows Subsystem for Linux (WSL 2) users an automated Xfce graphical desktop environment Win-KeX . This removes need for remote desktop clients or xClients or out of box scripts. Just typing in `kex` or clicking on the button, Win-KeX will give us a persistent-session GUI. <!--more-->

Install Win-KeX via: `sudo apt update && sudo apt install kali-win-kex`

Run Win-KeX via: `kex`

Stop Win-Kex via on WSL2 Terminal: `kex stop`

Stop Kali Desktop by pressing `F8` fn key and selecting _Exit Viewer_ option on the TigerVNC menu.

We can find more information about Win-Kex on [kali-docs](https://www.kali.org/docs/wsl/win-kex/) and [bleeping computer blog](https://www.bleepingcomputer.com/news/security/kali-linux-gets-a-gui-desktop-in-windows-subsystem-for-linux/).

> Win-Kex is only for WSL 2, please update your windows 10 version to support WSL2 and then the WSL version.

_One issue by running without any custom settings is that Tiger Vnc occupies fullscreen by default on all monitors, which could be removed in current session by disabling full screen mode on all monitors in options menu which is display on pressing `F8` Fn key. But this setting could not be stored for later GUI spawns_
